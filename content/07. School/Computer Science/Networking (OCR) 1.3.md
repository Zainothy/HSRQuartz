---
tags:
  - School
  - Computer-Science
  - Networking
aliases:
  - networks
  - OCR
  - GCSE
Topic: Networking
Completed: true
Links:
  - "[[Cyber Security OCR (1.4)]]"
  - "[[Systems Architecture (1.1)]]"
---


## Wired and Wireless Networks, Protocols and Layers (1.3.2):

### Wired:

Most wired networks consist of a multitude of devices that are all connected to a network switch. Every device is connected to a switch via a cable. Switches can be joined to form even larger networks. 

Most devices are connected to switches with [UTP Cables](https://isaaccomputerscience.org/concepts/net_hard_cables?examBoard=ocr&stage=gcse#utp), these are resilient to interference. 

The speed of a wired network is usually limited by the maximum speed that the [Ethernet Network](https://isaaccomputerscience.org/concepts/net_network_protocols?examBoard=ocr&stage=gcse#ethernet) can handle. For gigabit speeds a Cat-5e cable is required and a “gigabit network switch” is required. 

### Wireless:

Typically, Wireless Local Area Networks (WLAN) is based around a device called a [Wireless Access Point (WAP)](https://en.wikipedia.org/wiki/Wireless_access_point) . In typical homes, the WAP will be integrated into the device that your ISP has provided, normally known as a router. However, in larger buildings or corporations: there will be a multitude of discreetly placed WAP’s. 

Wireless Networks are useful and convenient because they allow for users to move around with their devices. On the other hand, they can be subject to interference from other signals and/or materials in the building blocking signals 

### Connecting to Wireless Networks:

In order for a connection to a Wireless Network to be established, you need to scan for networks within the range of your device. The range of a signal operating on 2.4ghz band is around 50m, it is much lower when operating on the faster 5ghz band. Networks will typically require passwords to be connected to, one that doesn’t have a password is an Open Network and is considered less secure as data is typically not encrypted.

## Hybrid Networks:

[Most Local Area Networks (LANs)](https://en.wikipedia.org/wiki/Local_area_network) have a combination of both wired and wireless connections. Wired will be used for more stationary devices, such as Desktop Computers or Printers. 

At home, you will probably have a network access device (commonly referred to as "the router") that is provided by your internet service provider (ISP). This device includes a wireless access point (WAP) for devices to connect to the network wirelessly and will also incorporate a small switch with a few Ethernet ports for wired connections.

In the average home, people will typically have a network access device ( referred to as a “router”) that is provided by your Internet Service Provider (ISP). It has an integrated WAP and a small switch to allow a few devices to have a hardwired connection. 

## Comparing Wired and Wireless:

| Factor  | Wired | Wireless |
| --- | --- | --- |
| Speed | Wired connections are typically faster as signals carried over a hardwire connection are less susceptible to interference  | As well as the introduction of interference, most wireless networks have layers of encryption. This introduces even more speed loss. |
| Security  | Wired networks are more secure. It is harder for hardwire connections to be tampered with or intercepted. | Wireless networks are less secure. Data can be intercepted by a 3rd party without the need for a physical connection.  |
| Range  | The range of a wired network is  greater, Copper cable can reliably carry signals for up to 100m and Fibre Optic can carry signals over 100km or more.  | The range of wireless signals is much lower as it can be obstructed/weakened easily by thick walls and obstacles. Therefore a mesh of access points is usually required to improve strength.  |
| Setup | Fixed cabling tends to be inflexible and therefore, if a layout is changed for a room the connection may not be in the desired placement  | Devices can be moved freely. They can be placed anywhere within range of the WAP  |
| Cost  | Wired networks can be expensive to setup. Hubs or Switches are required. In work environments they will need to be placed in a secure room or lockable cabinets to prevent tampering. Cables will need to be run through trunking to prevent health/safety issues and networks will need to be configured.  | Usually more than one WAP may be needed, especially if the building is large or made up of materials that may cause interference.  |

## Protocols and Layers:

### Layers of Protocols:

Modern communication systems are very complex and multiple organisations are involved in writing the software and developing the hardware that allows these devices to talk with each other. 

In order for communication systems to be open as possible, the different processes are divided up into layers, each layer has a defined responsibility. They are ordered in a way so that data moves from one layer to the next in its journey from the end-user to the network. 

The specification for how the interface between each layer works is documented well. This means all software engineers have to do is make sure that the data is in the correct format. The benefit of this is that there is independence for each layer from the others. For example, you can use the exact same browser regardless of whether you are connected through LAN or Mobile Data. 

## OSI Seven-Layer Model:

The OSI ( Open Systems Intercommunication) model: this was developed by the [International Organisation for Standardisation (ISO)](https://www.iso.org/home.html). In that model, all communications are split into seven different layers. 
## TCP/IP four-layer model:

The internet has an entirely separate model, it combines the physical and data link layers from the OSI model and turns them into a single link layer, it has a single application layer that is a combination of the application, presentation and session layers of the OSI model. 


This model may be confused with the TCP 5 Layer Model: In that, the physical and data link layers are separate.