# DAISI - Distributed AI Systems, Inc.
The DAISI system is build for the masses to use existing, available resources for AI Inference, code generation, tool execution, image generation, and more. 
The system should remain open and free to use, based on a simple credit system. Every time one of your hosts processes a token for someone else, you get a token that you can use in the future.

Apps, Skills, Tools, and Plugins will be made available through a marketplace in the future so that you can extend your Hosts and Private Networks however you choose. These may come at a fee,
which will be used to grow and support future development.

## Terminology
### Hosts
Hosts are the devices that process LLM, Tool, and generation requests using their own GPU/CPU setup. As you process requests for other people, you earn credit within that network, which you can later use for 
whatever purpose you choose. Hosts can be setup to allow for Direction Connections (DC) or to use Fully Orchestrated Connections (FOC). Either way, a session must be created via connection to the Orc, 
which is always validated by the Hosts so that unauthorized connections to the Host are prohibited.

### Orcs (Orchestrators)
Orcs coordinate the inference requests and act as a rally point for the Consumers and Hosts to connect anonymously to each other. All connections to public Orcs on the DAISI network will always
be using SSL. A network can have numerous Orc instances to process their requests and setup sessions. 

Hosts open a connection to Orcs when started and they communicate asynchronously via a system of queued commands. Consumers connect to Orcs via the SDK, requesting Hosts to process requests, at which time
the Orc will create a new Session for the Consumer to use for tools, inference, and more.

### Consumers 
Anyone that wants to process a request on the network is considered a Consumer. Usually, consumers will be an App that is created in the Manager that authenticates via the app's Secret Key, which is provided
in the Management Suite for the Orc.

### Network
Public and Private networks are possible in the Daisi system. Orcs can be setup to operate exclusively within a LAN on a private network that only allows Hosts within that network. In this way, intellectual property
and sensitive data can be protected within the boundaries of the currently LAN and not exposed to the public, unless desired.

## Security
Public networks should always be considered insecure, despite best efforts to enforce encryption, Trusted Security Environments (TEE), authentication, auhtorization, and other security measures. This is protect sensitive information from falling into nefarious hands. There's always a way should someone wish to be evil, so protect your systems and IP carefully.
