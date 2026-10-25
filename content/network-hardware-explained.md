# Network Hardware Explained: Modems, Routers, Switches, and Access Points

> **Module:** Hardware, Networks, and Behaviorist AI 
> **Level:** Beginner  
> **Estimated learning time:** 15–20 minutes  
> **Learning format:** Short reading, visual examples, and practice activities

## 1. Learning Objectives

After completing this lesson, learners should be able to:

- Identify four common network devices: modems, routers, switches, and wireless access points.
- Explain the main function of each device.
- Distinguish a router from a switch and a modem.
- Describe how network devices work together in a home or small office.
- Trace a basic connection from a personal device to the Internet.

## 2. Key Terms

| Term | Simple definition |
|---|---|
| Network | Two or more devices connected so they can communicate. |
| LAN | Local Area Network; a network within a limited area, such as a home, classroom, or office. |
| ISP | Internet Service Provider; a company that provides Internet access. |
| Modem | A device that connects to an ISP's access technology. |
| Router | A device that forwards IP packets between different networks. |
| Switch | A device that connects multiple wired devices within a LAN. |
| Access Point (AP) | A device that allows Wi-Fi devices to connect to a network. |
| IP address | A logical address used to identify a network interface for IP communication. |
| MAC address | A link-layer address used to identify a network interface on a local network. |
| Ethernet | A family of technologies commonly used for wired local networks. |

## 3. Why Do We Need Network Hardware?

Computers, smartphones, printers, and servers need a way to exchange information. Network hardware provides the connections and forwarding functions that make this possible.

Different devices perform different jobs. A switch connects devices inside a local network, a router forwards traffic between networks, and a wireless access point connects Wi-Fi devices to the network. A modem or optical network terminal (ONT) provides the connection to the Internet service, depending on the technology used.

Some home Internet devices combine several functions in one physical box. Therefore, one device may look like a router while also containing a modem, switch ports, and a wireless access point.

## 4. Four Important Network Devices

### 4.1 Modem or Optical Network Terminal (ONT)

![Example of a cellular modem and router](https://upload.wikimedia.org/wikipedia/commons/9/97/Modem_DirecTV_4G_LTE_Colombia.jpg?utm_campaign=index&utm_content=original&utm_source=commons.wikimedia.org)

*A real example of a cellular modem/router. Different Internet technologies use different equipment.*

A modem connects a customer's equipment to an Internet Service Provider (ISP) through a supported access technology. Depending on the service, it may convert signals so that the customer's network can communicate over the provider's connection.

Fiber-optic services commonly use an ONT to terminate the optical connection. A modem and an ONT are related in purpose, but they are not identical devices.

**Example:** A household has an Internet subscription. The service provider supplies a modem or ONT that connects the home equipment to its network.

**Remember:** A standalone modem does not necessarily provide Wi-Fi or connect multiple household devices by itself.

### 4.2 Router

![Home gateway and Wi-Fi router](https://upload.wikimedia.org/wikipedia/commons/c/c3/Home_Gateway_and_Wi-Fi_Router.jpg?utm_campaign=index&utm_content=original&utm_source=commons.wikimedia.org)

*A photograph of home gateway and Wi-Fi router equipment.*

A router connects different IP networks and forwards packets toward their destinations. It examines routing information to determine where traffic should go next.

In a typical home network, a router connects the local network to the ISP's network. Many home routers also provide Wi-Fi, DHCP address assignment, network address translation (NAT), and firewall features.

**Example:** Your laptop sends a request to a website outside your home network. The router forwards the traffic toward the Internet connection.

**Remember:** A router manages traffic between networks. A router does not have to include a modem or Wi-Fi access point.

### 4.3 Network Switch

![Network switches with Ethernet cables](https://upload.wikimedia.org/wikipedia/commons/e/e5/Network_switches.jpg?utm_campaign=index&utm_content=original&utm_source=commons.wikimedia.org)

*Network switches connect wired equipment through Ethernet cables.*

A switch connects multiple wired devices within a local network. It learns which MAC addresses are reachable through its ports and uses that information to forward Ethernet frames toward the appropriate destination.

Switches are useful when a classroom, laboratory, or office needs more wired network connections than the router provides.

**Example:** Four computers and a printer connect to one switch. The devices can communicate over the LAN when the network is configured correctly.

**Remember:** A basic switch connects devices within a LAN. It does not replace the router's role in connecting that LAN to other IP networks.

### 4.4 Wireless Access Point (AP)

![Wireless access point mounted on a wall](https://upload.wikimedia.org/wikipedia/commons/8/81/Access-point-wireless.jpg?utm_campaign=index&utm_content=original&utm_source=commons.wikimedia.org)

*A wireless access point provides Wi-Fi access to a network.*

A wireless access point allows Wi-Fi-enabled devices to join a network without using an Ethernet cable for the device's connection. It bridges wireless communication with the network's wired infrastructure.

Dedicated access points are common in schools, offices, and large buildings. In many homes, the access point is built into the Wi-Fi router.

**Example:** A smartphone connects to an office Wi-Fi access point and uses the local network to reach an online service.

**Remember:** Wi-Fi is a way to connect wirelessly. Having a Wi-Fi connection does not automatically mean that the Internet connection is working.

## 5. How Do These Devices Work Together?

![Example of a home local area network](https://upload.wikimedia.org/wikipedia/commons/a/ad/Home_LAN_local_area_network_example_diagram.png?utm_campaign=index&utm_content=original&utm_source=commons.wikimedia.org)

*Example of a home LAN showing wired and wireless devices, a router, and an Internet connection.*

Consider a small office with desktop computers, a printer, smartphones, and an Internet subscription.

A simplified network layout is:

    Internet
       |
    ISP connection
       |
    Modem or ONT
       |
    Router
       |
    Ethernet switch
       |---------------- Desktop computer
       |---------------- Network printer
       |
    Wireless access point
       ))) Smartphone
       ))) Laptop

This diagram shows separate devices for each function. Real networks may be arranged differently. For example, a Wi-Fi router may already include a switch and an access point, while an ISP gateway may combine the modem and router.

### Step-by-step explanation

1. The ISP provides the connection to the Internet.
2. The modem or ONT terminates the supported provider connection.
3. The router forwards traffic between the local network and other IP networks.
4. The switch connects wired devices within the local network.
5. The access point allows wireless devices to join the network.
6. The devices can communicate according to the network configuration and applicable security rules.

## 6. Comparison Table

| Device | Main job | Typical connection | Provides Wi-Fi? |
|---|---|---|---|
| Modem / ONT | Connects customer equipment to the ISP access service | Provider line to customer equipment | Not usually by itself |
| Router | Forwards traffic between IP networks | LAN and WAN/network connections | Sometimes |
| Switch | Connects wired devices within a LAN | Ethernet ports | No, not a basic Ethernet switch |
| Access point | Connects wireless devices to a network | Wi-Fi and a network uplink | Yes |

The functions may be combined in one physical device. Always distinguish the device's functions rather than relying only on its appearance.

## 7. Worked Example: Setting Up a Computer Lab

A computer lab has six desktop computers, one network printer, several student laptops, and an Internet subscription.

**Question:** Which devices are useful, and why?

**Solution:**

- **Modem or ONT:** Provides the connection to the ISP's access service.
- **Router:** Connects the lab's IP network to other networks, including the Internet.
- **Switch:** Provides enough Ethernet ports for the desktop computers and printer.
- **Wireless access point:** Allows student laptops to connect through Wi-Fi.

The router, switch, and access point may be separate devices or may have some functions combined. The final design depends on the equipment available and the network requirements.

## 8. Common Misunderstandings

**Misunderstanding 1: A modem and a router are the same thing.**

Correction: They perform different functions, although an ISP gateway may combine them.

**Misunderstanding 2: A switch connects a home directly to the Internet.**

Correction: A basic switch connects devices within a LAN. A router normally forwards traffic between the LAN and other IP networks.

**Misunderstanding 3: Every router provides Wi-Fi.**

Correction: Some routers are wired-only. Wi-Fi requires a wireless access point, which may be built into the router.

**Misunderstanding 4: If Wi-Fi is connected, the Internet must be working.**

Correction: A device may connect to the access point even when the ISP connection or another part of the network is unavailable.

## 9. Practice Activity

### Question 1

Which device primarily forwards traffic between different IP networks?

A. Switch  
B. Router  
C. Keyboard  
D. Monitor

### Question 2

A classroom needs to connect eight wired desktop computers to the same LAN. Which device is most directly suited to providing additional Ethernet ports?

A. Switch  
B. Modem  
C. Webcam  
D. Speaker

### Question 3

What is the main purpose of a wireless access point?

A. To store files permanently  
B. To process CPU instructions  
C. To allow wireless devices to connect to a network  
D. To replace every router

### Question 4

True or false: A device can connect to Wi-Fi even when the Internet service is unavailable.

### Question 5

A home has a modem, a router, and a switch. Explain the main job of each device in one sentence.

## 10. Answer Key

1. **B — Router.** It forwards IP packets between networks.
2. **A — Switch.** It connects multiple wired devices within a LAN.
3. **C — Wireless access point.** It provides wireless access to the network.
4. **True.** The local Wi-Fi connection may still work even when the external Internet connection fails.
5. **Example answer:** The modem connects the customer's equipment to the ISP access service, the router forwards traffic between networks, and the switch connects wired devices within the LAN.

## 11. Mini-Lecture Plan

**Suggested duration: 5 minutes**

- **Minute 1:** Introduce the problem: multiple devices need to communicate.
- **Minute 2:** Explain the modem/ONT and router using the photographs.
- **Minute 3:** Compare the switch and wireless access point.
- **Minute 4:** Trace the small-office network diagram.
- **Minute 5:** Ask learners to answer two practice questions and explain their reasoning.

## 12. Visual Design and Learning Adaptation

For a presentation or short video, use one main photograph per device and keep each explanation to two or three sentences.

A consistent visual key can help beginners remember the functions:

- **Modem / ONT:** Connection to the ISP.
- **Router:** Traffic between networks.
- **Switch:** Wired connections within the LAN.
- **Access point:** Wireless connections to the LAN.

Use arrows to show connection paths. Label each device with its function rather than only its name. The network diagram should remain readable when viewed on a presentation screen.

## 13. References

### Technical references

1. Cisco. *What Is a Switch vs. a Router?*  
   https://www.cisco.com/site/us/en/learn/topics/small-business/network-switch-vs-router.html

2. Cisco. *What Is an Access Point?*  
   https://www.cisco.com/site/us/en/learn/topics/small-business/what-is-an-access-point.html

3. Cloudflare. *What Is a Router?*  
   https://www.cloudflare.com/learning/network-layer/what-is-a-router/

### Image credits and licences

1. **Home gateway and Wi-Fi router photograph** — Project Kei. Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0).  
   https://commons.wikimedia.org/wiki/File:Home_Gateway_and_Wi-Fi_Router.jpg

2. **Network switches photograph** — ShakataGaNai. Creative Commons Attribution-ShareAlike 3.0 (CC BY-SA 3.0).  
   https://commons.wikimedia.org/wiki/File:Network_switches.jpg

3. **Wireless access point photograph** — Rodrigo César. Public domain, as released by the author.  
   https://commons.wikimedia.org/wiki/File:Access-point-wireless.jpg

4. **Cellular modem/router photograph** — JulianVilla26. Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0).  
   https://commons.wikimedia.org/wiki/File:Modem_DirecTV_4G_LTE_Colombia.jpg

5. **Home LAN diagram** — Sceeegt. Creative Commons CC0 1.0.  
   https://commons.wikimedia.org/wiki/File:Home_LAN_local_area_network_example_diagram.png

Check the licence and attribution requirements before redistributing or modifying each image. The photographs are examples of equipment; their physical appearance does not define every device of that type.
