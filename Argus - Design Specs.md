### Argus - Design Specs

A Modular and distributed web application scanner

---

#### Introduction

Argus is a **distributed** web application scanner written in golang. It uses a **modular** plugin based approach for scanner modules. This way, custom modules can be written with ease. It is written entirely in Golang and uses modern concurrency primitives to achieve an insanely fast speed.



An Argus configuration consits of a server and multiple agent nodes. The tool uses [nats-streaming-server](https://github.com/nats-io/nats-streaming-server) to manage communication between different nodes. Each node is very lightweight and uses very less memory and resources. 



#### Goals

- Distributed tooling allowing to scale very easily.
- Keeping server costs low while keeping performance to maximum.
- Fully modular allowing modules to be written in different languages like Javascript.

