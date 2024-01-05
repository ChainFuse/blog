---
authors:
    - demosjarco
categories:
    - ai
    - tech deep dive
date:
    created: 2023-10-26
---

I used ChatGPT to generate the TLS 3 way handshake diagram process used in https using mermaid

<!-- more -->

```mermaid
sequenceDiagram
autonumber
    participant Client
    participant Server

    Client->>Server: ClientHello
    note right of Server: Server processes ClientHello, generates keys, etc.
    Server->>Client: ServerHello
    note left of Client: Client processes ServerHello, generates keys, etc.
    Client->>Server: Key Exchange
    note right of Server: Server processes key exchange, finalizes handshake
```
