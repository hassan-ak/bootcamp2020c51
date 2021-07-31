# Intro to AWS Technologies With Cloud Development Kit (CDK)

## Class Notes: -

We previously used Netlify which is simple but lack functionality, it uses AWS lambda functions. Moving to AWS, concepts and APIs remains same but deployment changes.

Amazon started as an e-commerce store with a bunch of servers laying around in off peak hours so they started to rent out those servers. For a developer who doesn’t know upcoming traffic for a particular app can rent servers from a company and pay only for the use. Aws started from renting out servers and then added multiple services to it.

If we need to work with cloud services first, we need to understand what service to use and then learn, how to use and at time of use we combine multiple services. AWS combined all those services to a single platform and we can use all required services from a single source. This was used to be done by setting up a YML file with a disadvantage of too much coding. AWS introduced CDK to overcome this problem giving access to the developer for configuring these services using multiple high level coding language. CDK is made on top of cloud formation (where we need to write YML files) so when CDK projects are deployed firstly they are convert into cloud formation files and then AWS process it.

Three things to keep in mind PAAS (Google, AWS), IAAS(Machines) and SAAS (Applications --- charged when deployment). Abstraction is focusing on most important things to solve a problem. We will focus on serverless SAAS (Applications --- charged when used). SAAS are mostly multi tenancy apps. Multi tenancy means a single app available to multiple users (Daraz for sellers). We will be working with DApps (Decentralized) in future. These are apps which are built with the blockchain. DApps don’t send request to a single server but to blockchain and managed by multiple servers. Multi Cloud is another thing where multiple platforms are used for a single purpose.

There are client components in react and now working with CDK we have server components which are re-useable. All the configuration of CDK can be done with GI tools but not scale-able at all so doing it by using some language is preferred.
AWS account is required for development with CDK.
