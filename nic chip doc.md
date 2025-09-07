# NIC CHIPSET

This project is not going to be easy or intermediate. It is tough project and many people do this as a major project in their final year. 

Though we will not work on full fledged NIC in one go, we will make a NIC chip which could be feasible for a single person to achieve. 

---

# INDEX :

- [ ]  UNDERSTANDING WHAT NIC CHIPSET IS, AND HOW IT WORKS.
- [ ]  KEY REQUIREMENTS TO MAKE A NIC CHIP.

---

## NIC : NETWORK INTERFACE CARD

Network Interface card is a circuit that helps in receiving and transmitting data from internet to computer. It basically connects system to a network.

Data is transported in the form of analog signals through air or through port. This signal is then processed to digital by a NIC chip ( It is also known as LAN adapter/WAN adapter ). This signal is then transported to various parts of a computer to actually display the output as expected by a user. 

It also converts digital signals to analog and transport data through port to a network.

TERMINOLOGIES :

NODE/ENDPOINT : A device with which you need to communicate is known as NODE or ENDPOINT.

PACKETS : Small part of data to be tranmsitted with source and destinnation address.

FRAMES : Organised packet with header and trailer as DESTINATION and SOURCE addresses.

NETWORK MODELS : frameworks using which the process of digital communication take place.

There are frameworks that are used to model the communication in network.

TCP( TRANSMISSION CONTROL PROTOCOL )/IP( INTERNET PROTOCOL ) MODEL :

 It has four layers :

1. APPLICATION : The Application Layer is the top layer of the TCP/IP model and the one closest to the user. This is where all the apps you use like web browsers, email clients, or file sharing tools connect to the network. It acts like a bridge between your software (like Chrome, Gmail, or WhatsApp) and the lower layers of the network that actually send and receive data.
2. TRANSPORT : The Transport Layer is responsible for making sure that data is sent reliably and in the correct order between devices. 
3. NETWORK/INTERNET : The Internet Layer is used for finding the best path for data to travel across different networks so it can reach the right destination. 
4. NETWORK ACCESS : The Network Access Layer is the bottom layer of the TCP/IP model. It deals with the actual physical connection between devices on the same local network like computers connected by cables or communicating through Wi-Fi.

One of it’s goal is to make sure that the data sent by the sender arrives safely and correctly at the receiver’s end. To do this, the data is broken down into smaller parts called packets before being sent ( statement from geeksforgeeks ).

OSI ( OPEN SYSTEMS INTERCONNECION ) MODEL :

It is developed by INTERNATIONAL ORGANISATION OF STANDARDISTAION ( ISO ).

It consists of seven layers.

1. PHYSICAL LAYER : It is the bottom most layer of OSI. It is basically the hardware that is used to transmit data, either through ports , wired or wireless. It can convert signal from analog to digital or digital to analog.
2. DATA-LINK LAYER : 
    1. is the second layer from the bottom of OSI. It’s major is to ensure error free transmission of data.
    2. Also responsible for encoding, decoding, and organising the outgoing and incoming signals.
        1. It is divided into two sub layers : 1. **Logical Link Control (LLC)  |  2. Media Access Control (MAC)**
            1. LLC : This sublayer of the data link layer deals with multiplexing, the flow of data among applications and other services, and LLC is responsible for providing error messages and acknowledgments as well.
            2. MAC : MAC sublayer manages the device's interaction, responsible for addressing frames, and also controls physical media access. The data link layer receives the information in the form of packets from the Network layer, it divides packets into frames and sends those frames bit-by-bit to the underlying physical layer.
    

We will not dig deep into other layers as NIC  works in these two frames itself.

HERE ARE THE FUNCTIONS OD DATA LINK LAYER THAT NEEDS TO BE UNDERSTOOD. 

[![functions_of_data_link_layer_1.webp](functions_of_data_link_layer_1.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250128105254285850/functions_of_data_link_layer.webp)

[![functions_of_data_link_layer_2.webp](functions_of_data_link_layer_2.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250123162341626693/functions_of_data_link_layer_1.webp)

[![functions_of_data_link_layer_5.webp](functions_of_data_link_layer_5.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250123162341817996/functions_of_data_link_layer_2.webp)

[![functions_of_data_link_layer_6.webp](functions_of_data_link_layer_6.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250123164203841611/functions_of_data_link_layer_5.webp)

[![functions_of_data_link_layer_7.webp](functions_of_data_link_layer_7.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250123162342261043/functions_of_data_link_layer_6.webp)

[![functions_of_data_link_layer_8.webp](functions_of_data_link_layer_8.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250123162342455840/functions_of_data_link_layer_7.webp)

[![functions_of_data_link_layer_9.webp](functions_of_data_link_layer_9.webp)](https://media.geeksforgeeks.org/wp-content/uploads/20250123162342652878/functions_of_data_link_layer_8.webp)

https://media.geeksforgeeks.org/wp-content/uploads/20250123162342845770/functions_of_data_link_layer_9.webp

We can have wired/ wireless network Interface card. To keep the complexity to minimum, we will focus on building a wired NIC.

---

## KEY REQUIREMENTS :

( RPUGH IDEA )

Let us go step-by-step to know the requirements of makinng a NIC.

 You need ethernet cable to connect to a network. 

We need ethernet PHY : which converts digital signals to analog and analog signals to digital.

---

STEP 002: LEARN VERILOG AND P4.

STEP 003 : APPROACH CCC chairman, Mohit Tahilani sir.

He will be guiding in further process.

