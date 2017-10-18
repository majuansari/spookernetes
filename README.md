Spookernetes:




[ X ] Make [Traefik](https://docs.traefik.io/#docker) and Nginx work together

[ X ] Add Consul into the mix and find a way to make services discoverable during start up

[ X ] Print 'boo' and Container ID

[  X ] Include a header with the hostname of Nginx that serves the request

[  X ] Make Docker-Compose File K8s friendly

[ X  ] Using network policies, make it so only certain instances of Nginx can talk to certain PHP FPMs

[  x ] Deploy a single Nginx to show that it cannot talk to other things



Questions, Issues, etc:

What is [Container Runtime](http://programmableinfrastructure.com/components/container-runtime/):

- A container runtime allows users to manage resources like CPU and RAM, as well as start and stop containers, by providing
APIs and tooling that abstract the low level stuff. Simply put, it's an API that let's you interact with your containers.


What is CRI [(Container Runtime Interface)](http://blog.kubernetes.io/2016/12/container-runtime-interface-cri-in-kubernetes.html):

- CRI is a plugin API for containers built by Kubernetes meant to work with different types of containers.
This allows kubelet to work with whatever Container runtime you want and there will be no need to recompile.
CRI consists of protocol buffers and gRPC API, along with other things!

Wait, what's a [protocol buffer](https://developers.google.com/protocol-buffers/docs/overview)?

- Google made another thing, it's called a protocol buffer. Basically, it's a mechanism for serializing structured data.
"serializing structured data" - Okay, so serialization is the process of translating data into a format that can be stored (Think of serialized data in a database)
You define your data once (in a .proto file), and then you can have generated source code to write and read your structured data to and from different data streams and languages.

What's a [data stream](https://en.wikipedia.org/wiki/Data_stream):

-Packets

And [gRPC](https://grpc.io/docs/guides/)?

- So, RPC stands for remote procedure call, and this is how a program asks something to execute somewhere else, like a different computer.
gRPC is a framework that makes it so an application can call methods on different machines, but makes it seem like it's on the same machine.

What is Docker Swarm?

- Container Orchestration Tool

What is a Dockerfile?

- A [Dockerfile](https://docs.docker.com/engine/reference/builder/#format) is  file that contains commands to build images.
