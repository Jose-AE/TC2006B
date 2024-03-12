# Device Interconnection<!-- omit in toc -->

## Table of contents:<!-- omit in toc -->

- [OSI Model](#osi-model)
  - [Layer 1 (Physical)](#layer-1-physical)
  - [Layer 2 (Data Link)](#layer-2-data-link)
  - [Layer 3 (Network)](#layer-3-network)
- [IP Addressing](#ip-addressing)



<a id="com"></a>

## OSI Model

<img src="https://cf-assets.www.cloudflare.com/slt3lc6tev37/6ZH2Etm3LlFHTgmkjLmkxp/59ff240fb3ebdc7794ffaa6e1d69b7c2/osi_model_7_layers.png" alt="drawing" width="400"/>

### Layer 1 (Physical)

<blockquote>

<b>Transporting Bits</b>

The physical layer is responsible for the physical cable or wireless connection between network nodes. The physical layer contains information in the form of bits. When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together.  

- Examples
  - Coaxial Cable
  - Fiber Cable
  - Ethernet Cable
  - Wi-Fi
  - Hub
  - Modem

</blockquote>


### Layer 2 (Data Link)

<blockquote>

<b>Hop to Hop</b>

This layer reads and writes the bits from the physical connection, and it exists to take those bits from one NIC (Network Interface Card) to another.

**This layer uses the addressing scheme of MAC addresses**
- 48 Bits represented in 12 Hexadecimal digits 
- Example 94:65:9C:3B:8A:E5
- Every NIC has a unique MAC address 



**Technologies**
  - NIC (Network Interface Card)
  - Switches
  
**Functions of the Data Link Layer:**
- **Framing:** Framing is a function of the data link layer. It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.
- **Physical addressing:** After creating frames, the Data link layer adds physical addresses (MAC addresses) of the sender and/or receiver in the header of each frame.
- **Error control:** The data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.
- **Flow Control:** The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving an acknowledgment.
- **Access control**: When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.


</blockquote>


### Layer 3 (Network)

<blockquote>

<b>End to End</b>

The network layer works for the transmission of data from one host to the other located in different networks. It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available. The sender & receiver’s IP addresses are placed in the header by the network layer. 

**This layer uses the addressing scheme of MAC addresses**
- 48 Bits represented in 12 Hexadecimal digits 
- Example 94:65:9C:3B:8A:E5
- Every NIC has a unique MAC address 



**Technologies**
  - Router
  
**Functions of the Network Layer**
- **Routing:** The network layer protocols determine which route is suitable from source to destination. This function of the network layer is known as routing.
- **Logical Addressing:** To identify each device on Internetwork uniquely, the network layer defines an addressing scheme. The sender & receiver’s IP addresses are placed in the header by the network layer. Such an address distinguishes each device uniquely and universally.

</blockquote>


## IP Addressing


<blockquote>
An IP address, or Internet Protocol address, is a unique number assigned to every device (PC, mobile phone, router, etc.) on a computer network and used to communicate with each other and the internet.



**Structure of an IP address:**

The structure of an IP address depends on its version: IPv4 or IPv6. IPv4 is the most commonly used version of IP addresses and consists of a 32-bit binary number, composed of four groups of eight bits, separated by dots. Each section comprises one to three digits that fall between 0 and 255. Such a structure gives approximately 4.3 billion possible unique IPv4 addresses.

IPv6 is the most recent version of an IP address, initiated in 1995. It consists of eight groups of four hexadecimal digits separated by colons. Each digit represents four bits and allows for a much larger number of IPv6 combinations than IPv4.




Additionally, IP addresses are further categorized into two types:

- **Public IP Addresses:** These addresses are globally unique and routable on the public internet. They are assigned by Internet Service Providers (ISPs) or other internet authorities and are used to identify devices on the public internet.

- **Private IP Addresses:** These addresses are used for devices within a private network, such as a home or business network. They are not routable on the public internet and are used for internal communication within the confines of the private network. Commonly used private IP address ranges include those defined in RFC 1918, such as 10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16.

<img src="https://i.imgur.com/T7Tphnq.png">

</blockquote>

