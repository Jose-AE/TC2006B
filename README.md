# Device Interconnection<!-- omit in toc -->

## Table of contents:<!-- omit in toc -->

- [OSI Model](#osi-model)
  - [Layer 1 (Physical)](#layer-1-physical)
  - [Layer 2 (Data Link)](#layer-2-data-link)

<!--------------------------Time Complexity------------------------->

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

