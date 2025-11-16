---
{"dg-publish":true,"permalink":"/0-inbox/lsp/"}
---


# My Initial Understanding
I understand this as being a server that enriches the code editor with programming language specific functionalities and symbol indexing.

# What is LSP?
Also known as Language Server Protocol

This is a JSON-RPC-based communication protocol that is used between IDEs and servers that provide language intelligence tools. These tools include
- syntax highlighting
- code completion
- linting
- refactoring
- warning and error detection (similar to getting compilation errors before you compile the code? Unless the LSP compiles on your behalf and generates the errors?)

This is pretty open-source and once an LSP for a language is built, it can be used with any IDE that supports the protocol.

LSP was developed by [[Microsoft\|Microsoft]] back in 2016 and is now open source. The spec can be found in [[#^35ac2e|the official github repo]] 

With LSP, the code editor acts as a client to some LSP server (where is the LSP server hosted?)
LSP does not make any provisions about about how requests are transferred between client and server. Client and Server could be in the same process or on different machines.

## References
- https://microsoft.github.io/language-server-protocol/ - Official overview and specification of the protocol
- https://github.com/microsoft/language-server-protocol - Implementation of the protocol
{ #35ac2e}

-  https://langserver.org/ - for LSP implementations.



