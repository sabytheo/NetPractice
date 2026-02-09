_This project has been created as part
of the 42 curriculum by tsaby_

## **Description**

NetPractice is a general IT project in the 42 curriculum designed to introduce the fundamental concepts of networking. The goal of this project is to configure small-scale networks to ensure communication between specific devices.

The project utilizes a training interface where the user acts as a network administrator. Through a series of 10 levels, the user must manually configure:

IP addresses

Subnet masks

Default gateways

Routing tables

## **Instructions**

How to Run the Training Interface
The project is built to run in a web browser using a provided script.

* Open your terminal in the root of the repository you have downloaded by the profil page. The repository need to be extract.

*  Execute the script  ```./run.sh```

*  Select Training, and complete the field with your intranet login then Click on start.

*  Input the correct IP, Mask, or Route.

*  Once configured, click the on "Check" button.If the configuration is correct, the cables will turn green, indicating a successful connection.

*  If a level is completed successfully, you can click on the "Get my config" button one the interface to export a file (usually named levelX.json). you can now click on next level.

*  Complete all levels and ensure all configuration files are placed in the root of your git repository before pushing your project.

## **Resources**

This section lists the tools and documentation used to master the networking concepts required for this project.

 ### **TCP/IP Addressing**

**Definition**: TCP/IP (Transmission Control Protocol/Internet Protocol) is the foundational set of rules governing how data is exchanged over the internet.

*In NetPractice* : You focused specifically on IPv4 (Internet Protocol version 4). This is the unique numerical address assigned to every device (e.g., 192.168.1.1).

 ### **Subnet Masks**

**Definition** : A 32-bit number that masks an IP address and divides the IP address into the network address and the host address.

*In NetPractice* : This determines the size of the network. You likely used CIDR notation (e.g., /24, /30). You learned that a mask defines how many devices can fit in a network and that devices with different subnet masks (or overlapping subnets) cannot communicate correctly without routing

### **Default Gateways**

**Definition**: The IP address of the router interface that connects a local network to the rest of the world (or other networks).

*In NetPractice*: This is the "exit door." If a computer wants to send a packet to an IP outside its own subnet, it sends it to the Default Gateway. Without this configured, your device can talk to its neighbors, but not to the internet or other levels.

### **Routers and Switches**

These are the hardware devices that move data, but they operate at different "layers."

**Switch** (Layer 2 - Data Link): Connects devices within the same network (e.g., creating a LAN). It uses MAC addresses to direct traffic. In NetPractice, switches are often abstract, but they represent the cables connecting computers in a single group.

**Router** (Layer 3 - Network): Connects different networks together. It uses IP addresses to decide where to send packets. In NetPractice, you explicitly configured router interfaces to join two different subnets (e.g., connecting Subnet A to Subnet B).

### **OSI Layers (Open Systems Interconnection)**

**Definition** : A conceptual model that characterizes and standardizes the communication functions of a computing system without regard to its underlying internal structure and technology.

*In NetPractice*: You primarily worked with:

Layer 2 (Data Link Layer): Where Switches operate (dealing with local delivery).

Layer 3 (Network Layer): Where Routers, IP addresses, and Subnets operate (dealing with logical addressing and path determination).

### References & Tools

IP Calculation: [IP Subnet Calculator](https://www.calculator.net/ip-subnet-calculator.html) - Used to verify CIDR ranges.

### AI Usage Disclosure

In accordance with the project requirements, here is how AI tools were utilized during the development of this project:

**Concept Clarification**: AI was used to explain subnet mask and how they affect the number of available host addresses.

**Readme Generation**: AI was used to structure and format this README file to ensure it meets the formatting requirements.


