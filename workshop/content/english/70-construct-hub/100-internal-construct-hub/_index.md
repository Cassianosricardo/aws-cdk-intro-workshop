+++
title = "Internal Construct Hub"
weight = 200
bookFlatSection = true
+++

# Internal Construct Hub

So how do you go about sharing constructs with other members of your organization? There is the <a href="https://constructs.dev/" target="_blank">Construct Hub</a> but this is a public-facing website i.e. anyone in the world can access it. Perhaps your constructs are for internal Intellectual Property (IP) or as part of competetive research and development initiatives. It's likely against company policy to expose this type of information.

Lucky for you, the Construct Hub itself is a CDK Construct! This means you can deploy it in an AWS account and only allow access to internal resources. This way you can share your constructs with members of your team or organization without exposing them to the outside world.

![](./100-internal-construct-hub/internal-construct-hub.png)

To enable this functionality, you'll deploy the architecture shown in the above diagram.

There are typically 3 types of users who will leverage the Internal Construct Hub in some way:

1. Internal Construct Hub Administrators - These individuals are responsible for managing the Internal Construct Hub and the pipeline that deploys constructs to it.

2. Internal Construct Hub Producers - Developers who publish constructs to the Internal Construct Hub

3. Internal Construct Hub Consumers - Developers who will navigate to the Internal Construct Hub looking for helpful CDK constructs

The upcoming sections are mapped to the needs of these types of users. In the next section, we'll go through some initial setup before deploying the front-end of the Internal Construct Hub (The box labeled "Internal ConstructHub" in the diagram above).
