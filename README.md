# Serum on Akash

This is a guide to containerizing [Serum DEX](https://github.com/project-serum/serum-dex-ui) and deploying on [Akash](https://akash.network) in a non-custodial way. Akash is a permissionless and censorship-resistant cloud network that guarantees sovereignty over your data and your applications. With Akash, you’re in complete control of all aspects of the life cycle of an application with no middleman.

## Before We Begin

This is a technical guide, best suited to a reader with basic Linux command line knowledge. The audience for this guide is intended for includes:

* Application developers with little or no systems administration experience, wanting to deploy applications on the decentralized cloud.
* System administrators with little or no experience with infrastructure automation, wanting to learn more.
* Infrastructure automation engineers that want to explore decentralized cloud.
* Anyone who wants to get a feel for the current state of the decentralized cloud ecosystem.

You will need the below setup before we being:

1) Install Akash: Make sure to have Akash client installed on your workstation, check [install guide](https://docs.akash.network/guides/install) for instructions.
2) Choose Your Akash Network: You'll need to know information about the network you're connecting your node to. See [Choosing a Network](https://docs.akash.network/guides/version) for how to obtain any network-related information.
3) Fund Your Account: You'll need a AKT wallet with funds to pay for your deployment. See the [funding guide](https://docs.akash.network/guides/funding)
creating a key and funding your account.
4) Install Docker: You'll need docker running on your workstation, follow this [guide](https://docs.docker.com/get-docker/) to setup Docker on your workstation..
5) Setup Container Registry: To stage your containers to deploy onto Akash. We'll Docker Hub in this guide. [Signup](https://docs.docker.com/docker-hub/) for a free Docker Hub account if you haven't.