# OSI Layer Model

The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes how different systems communicate over a network. It breaks down network communication into seven distinct layers, each with its own specific responsibilities.

## The Seven Layers
<img width="5667" height="2834" alt="image" src="https://github.com/user-attachments/assets/3cf51d65-4cab-487f-b30c-ea71a2cfff2a" />

### Layer 7: Application Layer

This is the layer you interact with directly. When you're browsing websites, sending emails, or using any network application, you're working at the Application Layer. It's responsible for providing network services directly to your applications and acts as the window between the user and the network. This layer doesn't refer to the applications themselves, but rather the protocols and services that applications use to access the network.

### Layer 6: Presentation Layer

The Presentation Layer is like a translator that makes sure data is in a format that the receiving application can understand. It handles three main jobs: formatting data, encrypting it for security, and compressing it to save bandwidth. When you send an encrypted message or open a compressed file from the internet, the Presentation Layer is doing the heavy lifting to convert that data into something usable.

### Layer 5: Session Layer

Think of the Session Layer as a conversation manager. It establishes, maintains, and terminates communication sessions between applications. When two computers need to have an ongoing dialogue, this layer makes sure the conversation stays organized and coordinated. It handles the setup of the connection, keeps it running smoothly, and knows when to properly close it down.

### Layer 4: Transport Layer

The Transport Layer is all about reliable delivery. It ensures that data gets transferred accurately and completely between end systems. This layer breaks large messages into smaller segments, controls the flow of data so the receiver doesn't get overwhelmed, and detects and corrects errors that might occur during transmission. It's like a postal service that not only delivers your packages but also makes sure they arrive intact and in the right order.

### Layer 3: Network Layer

The Network Layer handles the logical addressing and routing of data across different networks. It works with IP addresses to determine the best path for data packets to travel from source to destination, even if they have to cross multiple networks to get there. This layer is like a GPS system that figures out the optimal route for your data to take through the complex web of interconnected networks that make up the internet.

### Layer 2: Data Link Layer

The Data Link Layer ensures error-free transmission of data frames between devices that are directly connected on the same network. It deals with physical addressing using MAC addresses (the unique identifier burned into your network card) and makes sure data frames are delivered correctly to the right device on the local network. This layer also handles error detection and can request retransmission if something goes wrong during the transfer.

### Layer 1: Physical Layer

At the bottom of the stack, the Physical Layer deals with the actual physical transmission of raw bits over the network medium. This includes the cables, connectors, electrical signals, radio frequencies, and light pulses that carry data. It's concerned with the nitty-gritty details like voltage levels, timing of signals, and the physical shape of connectors. Essentially, it's the layer that takes your digital data and converts it into physical signals that can travel across wires or through the air.

## How It All Works Together

Each layer communicates with the layers directly above and below it. When you send data, it travels down through all seven layers, with each layer adding its own information (headers) to help the corresponding layer on the receiving end do its job. When data is received, it travels back up through the layers, with each layer stripping off its header and processing the data before passing it upward. This systematic approach makes troubleshooting easier and allows different technologies and protocols to work together seamlessly.

## References

- Article - https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/
- Video - https://www.youtube.com/watch?v=vv4y_uOneC0
