# Intro to AWS Technologies With Cloud Development Kit (CDK)

## Overview

### Class Notes: -

We previously used Netlify which is simple but lack functionality, it uses AWS lambda functions. Moving to AWS, concepts and APIs remains same but deployment changes.

Amazon started as an e-commerce store with a bunch of servers laying around in off peak hours so they started to rent out those servers. For a developer who doesn’t know upcoming traffic for a particular app can rent servers from a company and pay only for the use. Aws started from renting out servers and then added multiple services to it.

If we need to work with cloud services first, we need to understand what service to use and then learn, how to use and at time of use we combine multiple services. AWS combined all those services to a single platform and we can use all required services from a single source. This was used to be done by setting up a YML file with a disadvantage of too much coding. AWS introduced CDK to overcome this problem giving access to the developer for configuring these services using multiple high level coding language. CDK is made on top of cloud formation (where we need to write YML files) so when CDK projects are deployed firstly they are convert into cloud formation files and then AWS process it.

Three things to keep in mind PAAS (Google, AWS), IAAS(Machines) and SAAS (Applications --- charged when deployment). Abstraction is focusing on most important things to solve a problem. We will focus on serverless SAAS (Applications --- charged when used). SAAS are mostly multi tenancy apps. Multi tenancy means a single app available to multiple users (Daraz for sellers). We will be working with DApps (Decentralized) in future. These are apps which are built with the blockchain. DApps don’t send request to a single server but to blockchain and managed by multiple servers. Multi Cloud is another thing where multiple platforms are used for a single purpose.

There are client components in react and now working with CDK we have server components which are re-useable. All the configuration of CDK can be done with GI tools but not scale-able at all so doing it by using some language is preferred.
AWS account is required for development with CDK.

## Get AWS Account

- [AWS Educate](https://aws.amazon.com/education/awseducate/)
- [AWS Free Tier](https://aws.amazon.com/free/)
- [GitHub Student Pack](https://education.github.com/pack)

## Reading Material: -

Base Technology Stack

1. Frontend: React with Typescipt and Storybook
2. Infrastructure As Code and Automation Tools: AWS CDK
3. Integration: AWS EventBridge
4. Computing: AWS Lambda
5. Programing Language: TypeScript
6. Orchestration: AWS Step Functions
7. CDN: Amazon CloudFront
8. Static Content: Amazon S3
9. API Front End: GraphQL using AWS AppSync
10. Database: AWS DynamoDB, AWS Arora Serverless, and AWS Neptune
11. Container Management: Fargate
12. Observability: AWS X-Ray
13. IDE: VS Code
14. CI/CD: Github Actions
15. Version Control: GitHub

Useful Links

- [The Serverless Future of Supercharged Applications](https://containerjournal.com/topics/container-ecosystems/the-serverless-future-of-supercharged-applications/)
- [The impact of serverless on the future of cloud technology](https://cio.economictimes.indiatimes.com/news/cloud-computing/the-impact-of-serverless-on-the-future-of-cloud-technology/77275273)
- [It is the future](https://www.devopsonline.co.uk/is-serverless-the-future/)
- [Cloud 2.0: Serverless architecture and the next wave of enterprise offerings](https://www.mckinsey.com/business-functions/mckinsey-digital/our-insights/tech-forward/cloud-20-serverless-architecture-and-the-next-wave-of-enterprise-offerings)
- [Why Serverless is Cloud 2.0](http://serverlesscomputing.london/wp-content/uploads/2019/06/Paul-Johnston-Why-Serverless-is-Cloud-2.0.pdf).
- "In a recent informal poll, more than 66% of developers chose AWS CDK as their technology of choice for building serverless applications on AWS."
- [The CDK Patterns open source journey](https://aws.amazon.com/blogs/opensource/the-cdk-patterns-open-source-journey/)
- In this repo we have used TypeScript for CDK development. Because we consider it the best language for CDK the reason are listed in this [article](https://awsmaniac.com/which-programming-language-is-the-best-for-aws-cdk/). Application and Business code in the steps is implemented in both Typescript and Python.

## AWS CDK

[AWS CDK](https://github.com/aws/aws-cdk) is an open source software development framework to model and provision your cloud application resources using familiar programming languages. With AWS CDK, you can define your infrastructure as code and provision it through AWS CloudFormation. AWS CDK is available to use in all AWS regions. In this learning repo we will use CDK with TypeScript.

[CDK Primer](https://www.aws.training/Details/Curriculum?id=64511)

[Why Amazon Is Bullish on AWS Cloud Development Kit](https://www.datacenterknowledge.com/amazon/why-amazon-bullish-aws-cloud-development-kit)

[What is the AWS CDK?](https://docs.aws.amazon.com/cdk/latest/guide/home.html)

We expect that Open Source AWS CDK will become the defacto standard for Infrastructure as Code (IAC) not just for AWS but other clouds as well. Thus becoming the standard IAC multicloud tool. It is already available for [Terraform](https://github.com/hashicorp/terraform-cdk) and [Kubernetes](https://cdk8s.io/). CDK has already become the de facto software development framework internally at AWS. AWS CDK is DevOps for Developers and is the Ultimate DevOps tool.

[Infrastructure as Code: What Is It? Why Is It Important?](https://www.hashicorp.com/resources/what-is-infrastructure-as-code)

[AWS CDK API Reference](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html)

Alternatives

[Pulumi vs CDK](https://www.pulumi.com/docs/intro/vs/cloud_template_transpilers/)

[Serverless Framework vs CDK](https://www.secjuice.com/aws-cdk-vs-serverless-framework/)

[CloudFormation, Terraform, or CDK? A guide to IaC on AWS](https://acloudguru.com/blog/engineering/cloudformation-terraform-or-cdk-guide-to-iac-on-aws)

[Will AWS CDK replace Terraform and the Serverless Framework?](https://blog.codecentric.de/en/2019/09/aws-cdk-versus-terraform-and-serverless-framework/)

[Amplify vs CDK](https://stackoverflow.com/questions/60087064/aws-cdk-vs-aws-amplify#:~:text=Amplify%20is%20ok%20for%20deploying,deploy%20static%20sites%20with%20CDK.)

[SAM vs CDK](https://aws.amazon.com/cdk/faqs/#:~:text=AWS%20CDK%20offers%20broad%20coverage,Python%2C%20C%23%2C%20and%20Java.&text=If%20you%20prefer%20defining%20your,SAM%20is%20the%20better%20fit.)

[Awesome CDK](https://github.com/kolomied/awesome-cdk)

## Event-Driven Architecture

[What is an Event-Driven Architecture?](https://aws.amazon.com/event-driven-architecture/)

[Operating Lambda: Design principles in event-driven architectures – Part 2](https://aws.amazon.com/blogs/compute/operating-lambda-design-principles-in-event-driven-architectures-part-2/)

[BUILDING EVENT-DRIVEN ARCHITECTURES WORKSHOP ON AWS](https://event-driven-architecture.workshop.aws/)

[10 Things Serverless Architects Should Know](https://aws.amazon.com/blogs/architecture/ten-things-serverless-architects-should-know/)

[What a typical 100% Serverless Architecture looks like in AWS!](https://medium.com/serverless-transformation/what-a-typical-100-serverless-architecture-looks-like-in-aws-40f252cd0ecb)

[EventBridge: The key component in Serverless Architectures](https://medium.com/serverless-transformation/eventbridge-the-key-component-in-serverless-architectures-e7d4e60fca2d)

[How to Use Amazon EventBridge to Build Decoupled, Event-Driven Architectures](https://pages.awscloud.com/AWS-Learning-Path-How-to-Use-Amazon-EventBridge-to-Build-Decoupled-Event-Driven-Architectures_2020_LP_0001-SRV.html)

[Rethinking Serverless Architectures With Eventbridge](https://blog.thundra.io/rethinking-serverless-architectures-with-eventbridge)

[Architecting Serverless Solutions (Must Do this Course)](https://www.aws.training/Details/eLearning?id=42594)

[Introduction to Messaging for Modern Cloud Architecture](https://aws.amazon.com/blogs/architecture/introduction-to-messaging-for-modern-cloud-architecture/)

[Moving to event-driven architectures](https://www.youtube.com/watch?v=h46IquqjF3E)

[Deep Dive on Amazon EventBridge - AWS Online Tech Talks](https://www.youtube.com/watch?v=28B4L1fnnGM)

[Integrating Amazon EventBridge into your serverless applications](https://aws.amazon.com/blogs/compute/integrating-amazon-eventbridge-into-your-serverless-applications/)

[Rethinking Serverless Architectures With Eventbridge](https://blog.thundra.io/rethinking-serverless-architectures-with-eventbridge)

[Deep Dive on Amazon EventBridge](https://pages.awscloud.com/Deep-Dive-on-Amazon-EventBridge_2019_0919-SRV_OD.html)

## CDK Construction Zone: For Advanced CDK Users Directly From the CDK Team

[CDK construction zone | S1 Ep 1](https://m.twitch.tv/videos/916591005)

## Learning Repository

- [Learn Full Stack Serverless Apps and API Development with CDK in Baby Steps](https://github.com/panacloud-modern-global-apps/full-stack-serverless-cdk)

## Video Lecture

[Werner Vogels on the AWS Cloud Development Kit (AWS CDK)](https://www.youtube.com/watch?v=AYYTrDaEwLs)

- [YouTube English](https://www.youtube.com/watch?v=bnTCwunqhMc)
- [Facebook English](https://www.facebook.com/zeeshanhanif/videos/10225155745305611)
- [YouTube Urdu](https://www.youtube.com/watch?v=JhFiu-krGZI)
- [Facebook Urdu](https://www.facebook.com/zeeshanhanif/videos/10225164884934096)
