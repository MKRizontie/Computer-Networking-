# Computer-Networking-
This repository serves as a comprehensive guide to computer networking, covering fundamental concepts, protocols, and advanced topics. It is designed for beginners, students, and professionals seeking to strengthen their understanding of networking principles.
What is Networking? 1
What is Networking?
Networking is like building roads that connect houses (computers) so they can send messages (data) to
each other. Imagine two friends living in different neighborhoods want to send letters. They need a system
of streets, addresses, and rules for how to send and receive mail. Thats what a network does for
computers.
How Networks are Built
Networks can be built in different shapes (topologies):
Star: Like a mall where all shops are connected to a central hall.
Mesh: Like a spiderweb where every point connects to others.
Tree: Like branches of a tree with one main trunk and smaller branches.
They also use different tools to connect (mediums):
Ethernet cables: Like roads.
Fiber optics: Like high-speed highways.
Wireless Wi-Fi): Like sending letters using drones.
And they follow different rules (protocols):
TCP Like making sure a package is delivered safely and signed for.
UDP Like shouting a message without caring if someone heard it.
Why Security in Networking Matters
Think of your network as your house:
A flat network is like living in a house with just one lock on the door. Its easy for someone to break in
and roam around without restrictions.
A segmented network is like having separate rooms with locks, alarms, and cameras. Even if
someone gets in, they cant access everything.
Examples for Better Security
 Access Control Lists ACLs):
Imagine putting a fence around your yard with gates for entry and exit. If someone tries to jump over
the fence, its suspicious and easier to notice.
Example: Why is the printer talking to the server over HTTP (an unsecure method)?
 Documentation and Monitoring:
Think of putting lights around your yard to see whats happening.
Example: Why is the printer talking to the internet at all?
 Intrusion Detection Systems:
Like having bushes near your windows. They make it harder for someone to sneak in and easier to
detect unusual activity.
Example: Why did a port scan come from the printer network?
What is Networking? 2
Common Mistakes
Many people make their networks too simple and flat (one big space with no divisions). This is like letting
every visitor in your house go to any room without checking where they belong.
For example:
You give your printer an address IP on a flat network. Now the printer can talk to your servers,
computers, and even the internet without restriction. Thats risky!
Story Time: A Pentesters Mistake
A penetration tester (like a burglar hired to test your locks) made this mistake:
The company had split its network into two halves:
One for servers: 10.20.0.110.20.0.126
One for client devices: 10.20.0.12910.20.0.254
The tester's computer was set to talk to everyone (flat network) but could only communicate with client
devices. They missed the fact that the servers were on a different "room" (network segment).
How the Internet Works (Simple Analogy)
Your home network Wi-Fi): Like your house with its own mailbox (router).
The internet: Like a massive delivery system with post offices ISPs) everywhere.
Sending a request:
When you type a website like "www.hackthebox.eu," its like writing a letter with an address.
Your router sends the letter to the ISP, which finds the actual "geographical" address IP address).
The website responds, and the packet (data) is delivered back to you.
Making Networks More Secure
 Separate Networks Segmentation):
Divide devices into smaller networks based on their purpose:
Web servers in a DMZ Demilitarized Zone): Like keeping visitors in a guest room instead of the
living room.
Workstations isolated: Prevents employees computers from talking to each other unnecessarily.
 Admin Network:
Protect routers and switches by keeping them on their own private network.
Example: This stops hackers from sending fake instructions (man-in-the-middle attacks).
 Dedicated Networks for Phones/Printers:
Phones need special treatment to avoid delays (like giving ambulances priority on roads).
Printers are hard to secure and can be used to steal passwords. Keep them on their own network.
Takeaway
Think of your network as a neighborhood:
A flat network is like having one giant open field with no fences or walls—risky!
What is Networking? 3
A segmented network is like having houses, fences, and security cameras. Each part has its purpose,
making it harder for intruders to roam freely.
When you design or manage a network, always think about:
Who should talk to whom?
How can you make it hard for attackers to move around?
What tools can help detect suspicious activity?
Networking connects devices so they can talk to each other, like roads connecting towns or
neighborhoods. Depending on how far the network stretches or how it is set up, we give them different
names.
There are two main categories to know:
Common Terms: These are practical terms youll hear often.
Book Terms: These are terms that are good to know for exams or rare cases.
Common Terminology
Network Type Definition
Wide Area Network WAN
The Internet or any large network that connects smaller networks together.
Example: Government networks.
Local Area Network LAN A small network, like your home or office network.
Wireless Local Area Network
WLAN
A LAN that works over Wi-Fi instead of cables. Example: Your home Wi-Fi.
Virtual Private Network VPN
A secure tunnel to connect devices or networks over the internet. Example: Remote
work networks.
Breakdown of Common Terms
WAN (Wide Area Network)
A WAN connects multiple LANs together. The Internet is the most common example of a WAN.
Think of it as: Highways connecting different cities LANs).
Example: Your home network is connected to the Internet WAN through your Internet Service
Provider ISP.
Other WANs: Large companies and governments often have private WANs (e.g., Intranets).
LAN/WLAN (Local Area Network/Wireless Local Area Network)
A LAN connects devices within a small area, like your home or office. If its wireless, its called a WLAN.
Think of it as: Streets in your neighborhood.
Example: Your laptop, phone, and smart TV all connected to your Wi-Fi.
Key Fact: LANs typically use private IP addresses like 192.168.x.x or 10.x.x.x, which cannot be
accessed directly from the Internet.
VPN (Virtual Private Network)
A VPN creates a secure connection between devices or networks over the Internet. It makes you feel like
youre connected to a private network even if youre far away.
What is Networking? 4
Think of it as: A secret tunnel between two places.
Types of VPNs:
 Site-to-Site VPN Connects two networks, like linking two offices in different cities.
Example: Two company branches in New York and London sharing files securely.
 Remote Access VPN Lets individual devices connect to a network.
Example: Hack The Boxs VPN lets you connect to its labs from anywhere.
 SSL VPN Works in your browser, streaming applications or desktops securely.
Example: Hack The Box Pwnbox.
Split-Tunnel VPNs: Only some traffic goes through the VPN (like Hack The Box labs), while the rest
uses your regular Internet.
Full-Tunnel VPNs: All your traffic goes through the VPN, which is better for security.
Book Terms
Network Type Definition
Global Area Network GAN
A worldwide network. Example: The Internet or private networks of global
companies.
Metropolitan Area Network MAN
Connects multiple LANs in a city or region. Example: A citys government
network.
Personal Area Network PAN
A very small network for personal devices. Example: Your phone connected to
your smartwatch.
Wireless Personal Area Network
WPAN
A wireless version of a PAN. Example: Devices connected via Bluetooth.
Breakdown of Book Terms
GAN (Global Area Network)
A GAN connects devices and networks globally.
Think of it as: The entire world connected by undersea cables, satellites, and data centers.
Example: The Internet or a global companys private network.
MAN (Metropolitan Area Network)
A MAN connects multiple LANs in a city or region.
Think of it as: Express trains connecting stations LANs) in a city.
Example: A city governments network connecting schools, libraries, and offices.
PAN/WPAN (Personal Area Network/Wireless Personal Area Network)
A PAN connects devices around one person, like a phone and smartwatch. A WPAN is the wireless
version, often using Bluetooth.
Think of it as: A tiny bubble around you for your devices.
Example: Your wireless headphones connected to your phone via Bluetooth.
Real-Life Example: Smart Homes with IoT
What is Networking? 5
In smart homes, WPANs are used to connect low-power devices like smart bulbs, thermostats, and
doorbells. They use protocols like ZigBee or ZWave to communicate with each other.
Think of it as: A mini-network in your house for controlling devices.
Example: Turning off the lights or locking the door from your phone.
Conclusion
Networking comes in all shapes and sizes, from small personal networks PAN to global ones GAN.
Heres the summary:
WAN Internet or large networks connecting LANs.
LAN/WLAN Small networks at home or office (wired or wireless).
VPN Secure tunnels to connect devices or networks.
GAN/MAN Large-scale networks for cities or globally.
PAN/WPAN Tiny networks for personal devices like Bluetooth headphones.
Each type serves a different purpose, but together, they make up the world of networking!
What is Network Topology?
Network topology describes how devices (like computers and routers) are connected and interact within a
network. It can be physical (how devices are physically linked with cables or wireless signals) or logical
(how data flows across the network).
Think of it as:
Physical topology: The map of roads connecting cities.
Logical topology: The rules for how traffic moves on those roads.
Key Parts of Network Topology
Network topology has three main aspects:
 Connections
 Nodes Devices)
 Classifications Types)
1. Connections
This describes the method used to link devices in a network.
Wired Connections Wireless Connections
Coaxial cabling Wi-Fi
Glass fiber cabling Cellular 4G, 5G
Twisted-pair cabling Ethernet) Satellite
Example:
A wired Ethernet connection at home uses twisted-pair cables.
Wi-Fi or cellular networks are wireless connections.
2. Nodes (Devices)
Nodes are the points where devices connect to the network. They send, receive, or forward data.
What is Networking? 6
Examples of Network Nodes Functions
Repeaters Boost weak signals to travel longer distances.
Hubs Broadcast data to all devices in a network.
Switches Direct data to the correct device.
Routers/Modems Manage traffic between different networks.
Gateways Connect different network types.
Firewalls Protect networks from unauthorized access.
Example:
Your router at home is a node that connects your devices to the Internet.
A switch in an office connects many computers in a LAN.
3. Classifications (Types of Topology)
Network topology can be physical (how devices are connected) or logical (how data flows).
Here are the 8 basic types of topologies:
Type Description
Point-to-Point Direct connection between two devices.
Bus All devices share a single cable.
Star All devices connect to a central hub, switch, or router.
Ring Devices are connected in a circle; data flows in one direction.
Mesh Devices connect directly to multiple others; can be fully or partially connected.
Tree Like a hierarchical structure; combines multiple star topologies.
Hybrid Mix of different topologies (e.g., star and bus).
Daisy Chain Devices are connected one after another in a line.
Detailed Explanation of Topologies
1. Point-to-Point Topology
What it is: A simple connection between two devices.
Think of it as: A direct phone line between two people.
Example: A computer connected directly to a printer.
2. Bus Topology
What it is: All devices share the same cable. Data travels along this single path.
Think of it as: A shared microphone where only one person can talk at a time.
Example: Early Ethernet networks using coaxial cables.
3. Star Topology
What it is: All devices connect to a central device (like a switch or router).
Think of it as: A wheel with spokes connecting to a central hub.
Example: Most home networks where all devices connect to a Wi-Fi router.
Advantage: Easy to add or remove devices.
What is Networking? 7
Disadvantage: If the central device fails, the network stops working.
4. Ring Topology
What it is: Devices are connected in a circle, and data travels in one direction.
Think of it as: A relay race where the baton (data) passes around in a loop.
Example: Token Ring networks used in the past.
Advantage: Easy to predict data flow.
Disadvantage: If one connection breaks, the entire network fails.
5. Mesh Topology
What it is: Devices connect to multiple others for redundancy. Can be fully connected (every device
links to every other) or partially connected.
Think of it as: A web where multiple paths exist between points.
Example: The Internet or a WAN with backup links.
Advantage: High reliability; if one connection fails, data can take another path.
Disadvantage: Complex and expensive to set up.
6. Tree Topology
What it is: Combines multiple star networks into a hierarchical structure.
Think of it as: A family tree with branches.
Example: A company network where departments are star networks connected to a central backbone.
Advantage: Scalable for large networks.
Disadvantage: A single failure in the backbone can affect the entire network.
7. Hybrid Topology
What it is: A mix of two or more topologies.
Think of it as: Combining different building blocks into one system.
Example: A tree topology connecting star networks over a bus.
Advantage: Flexible to meet specific needs.
Disadvantage: Can be complex and expensive to manage.
8. Daisy Chain Topology
What it is: Devices are linked in a straight line.
Think of it as: Christmas lights, where one bulb connects to the next.
Example: Automation networks like CAN in manufacturing.
Advantage: Simple to set up for small networks.
Disadvantage: If one device fails, it can disrupt the entire chain.
Conclusion
What is Networking? 8
Network topologies determine how devices are connected and communicate. Here's a quick summary:
Point-to-Point: Simple and direct.
Bus: Shared single cable; easy but outdated.
Star: Common for home and office networks.
Ring: Sequential but prone to failure.
Mesh: Reliable with multiple paths but costly.
Tree: Hierarchical for large setups.
Hybrid: Flexible for complex needs.
Daisy Chain: Linear connections, simple but fragile.
Choosing the right topology depends on the size, purpose, and budget of your network.
What is a Proxy? (Simplified Version)
A proxy is like a middleman that sits between two parties—like you and the internet. Its job is to pass
messages back and forth while possibly inspecting, filtering, or changing them along the way.
Think of it as a receptionist in an office. You tell the receptionist what you need, and they communicate
your request to the right department. Similarly, a proxy handles your request to access something online
and decides how to process it.
Different Types of Proxies (with Real-Life Examples)
1. Forward Proxy
What it does Acts on behalf of the user (you) to connect to something online.
Example You want to visit a website, but you're on a school or work network that uses a proxy. The
proxy fetches the website for you but might block certain sites based on rules, like banning social
media.
Analogy Imagine sending a letter to someone. Instead of mailing it directly, you give it to a friend who
mails it for you.
Real-Life Use Case:
Companies use forward proxies to prevent employees from accessing harmful or unproductive
websites.
Tools like Burp Suite act as a forward proxy to help cybersecurity professionals test websites by
intercepting and analyzing web traffic.
2. Reverse Proxy
What it does Acts on behalf of the service (like a website or server) to protect it or manage traffic.
Example When you visit a popular site like Amazon, youre not connecting directly to Amazons
servers. Instead, a reverse proxy (like Cloudflare) handles your request, checks for security threats,
and forwards it to Amazons server if its safe.
Analogy Imagine calling a famous celebritys office. You dont speak directly to them; their assistant
answers and forwards your message to the celebrity if appropriate.
Real-Life Use Case:
What is Networking? 9
Organizations use Cloudflare as a reverse proxy to block malicious traffic (e.g., bots or hackers)
and handle Distributed Denial of Service DDoS attacks.
3. Transparent Proxy
What it does Works without you knowing its there. It doesnt require special settings on your device.
Example When you use free Wi-Fi at a coffee shop, a transparent proxy might filter or monitor the
sites you visit to block inappropriate content.
Analogy Its like a security guard at a mall quietly observing shoppers to ensure theyre following the
rules.
Real-Life Use Case:
Hotels and schools often use transparent proxies to enforce their internet usage policies.
4. Non-Transparent Proxy
What it does Requires you to configure your device or software to use it.
Example If your office network requires you to set up proxy settings in your browser to access the
internet, thats a non-transparent proxy.
Analogy This is like having to knock on a specific door and announce yourself before entering a
building.
Real-Life Use Case:
Developers configure non-transparent proxies to debug network traffic or simulate different
internet conditions.
Common Misconceptions About Proxies
 "Proxies VPNs"
A VPN changes your location and encrypts your data but doesnt act as a mediator for inspecting
traffic. Most people confuse the two because both can hide your IP address.
 "Proxies are only for hackers or illegal activities"
While hackers use proxies to hide their identity, proxies are widely used for legal purposes, like
speeding up website performance or improving network security.
Everyday Examples to Understand Proxies Better
Netflix:
If Netflix isnt available in your country, you might think a “proxy lets you watch shows from
another country. Technically, thats usually a VPN, not a proxy, but the idea of rerouting your
connection applies to both.
School Networks:
When a school blocks YouTube, its likely using a forward proxy to filter web traffic.
Customer Support Call Centers:
If you call a support hotline, the person who answers is like a reverse proxy—they listen to your
request and forward it to the right department.
The Key Idea
What is Networking? 10
A proxy sits in the middle of your connection to do something useful—filter, inspect, or protect. Whether
its helping you access a website, securing a server, or monitoring your network, its like a middleman that
makes communication smoother (or safer) depending on its type.
Understanding the OSI and TCP/IP Models in Simple Terms
The OSI Open Systems Interconnection) and TCP/IP Transmission Control Protocol/Internet Protocol)
models describe how data moves from one computer to another. They break the communication process
into layers, with each layer responsible for specific tasks. Think of them like a factory assembly line: each
station (layer) has its job to ensure the product (data) reaches its destination in perfect condition.
The OSI Model: 7 Layers of Communication
The OSI model divides the process into seven layers, from the physical transfer of data (electric signals,
light, etc.) to the meaningful messages humans understand. Here's a simple breakdown:
 Physical Layer
What it does Transfers raw bits 0s and 1s) over cables, Wi-Fi, or other media.
Example The actual Ethernet cable or Wi-Fi signal you use.
Analogy It's like the roads and vehicles used to deliver goods.
 Data Link Layer
What it does Organizes raw data into frames for transmission and ensures error-free delivery.
Example A switch or MAC address managing your connection.
Analogy Think of this as traffic rules ensuring cars (data) dont crash.
 Network Layer
What it does Handles addressing and routing so data knows where to go.
Example An IP address directing packets to the right device.
Analogy Its like GPS guiding a car to its destination.
 Transport Layer
What it does Manages data delivery, ensuring its complete and in order.
Example TCP and UDP protocols controlling the flow.
Analogy This is like packaging goods in boxes to ensure nothing gets lost.
 Session Layer
What it does Manages and maintains connections between devices.
Example Logging into a website and staying connected.
Analogy Think of this as scheduling a meeting room for a conversation.
 Presentation Layer
What it does Translates data formats so devices understand each other.
Example Converting video formats or encrypting data.
Analogy This is like translating languages for two people to communicate.
 Application Layer
What it does Where humans interact with the network.
Example Web browsers HTTP, email SMTP, or file transfers FTP.
What is Networking? 11
Analogy This is like the customer receiving their package.
The TCP/IP Model: 4 Simplified Layers
The TCP/IP model is a practical approach used on the Internet today. It combines some OSI layers to
simplify the process. Its like a shortcut map:
 Network Interface Similar to OSIs Physical Data Link Layers)
Handles physical connections and data framing.
Example: Ethernet or Wi-Fi protocols.
 Internet Similar to OSIs Network Layer)
Manages IP addresses and routing data.
Example: IPv4, IPv6.
Analogy: Ensures the package gets to the correct address.
 Transport Same as OSIs Transport Layer)
Ensures data delivery and order.
Example: TCP (reliable) or UDP (fast but less reliable).
 Application Combines OSIs Application, Presentation, and Session Layers)
Where humans interact with the network services.
Example: HTTP, FTP, DNS.
How Data Travels (Encapsulation and Decapsulation)
When data moves from your computer to another device:
 It starts at the Application Layer, where you send a message (e.g., a web request).
 As the message moves down the layers, each adds its own header (extra information) to guide it, like
adding labels to a package. This is called encapsulation.
 At the receiving device, the process reverses. Each layer reads and removes its header, like
unwrapping a gift, in a process called decapsulation.
Real-Life Analogy: Ordering a Pizza
Lets compare this process to ordering a pizza:
 Application Layer You place an order with the pizza shop (e.g., by calling or using an app).
 Transport Layer The shop confirms your order and prepares the pizza, ensuring its complete.
 Network Layer The delivery driver gets your address and plans the route.
 Data Link Layer The driver follows the traffic rules to reach your house.
 Physical Layer The pizza is handed to you.
Why Both Models Matter to Penetration Testers
TCP/IP Model Gives a high-level overview of how devices communicate. Useful for quickly
understanding network setups and spotting weak points.
OSI Model Allows for detailed analysis of each step, helping to identify specific vulnerabilities, like
issues in encryption or routing.
What is Networking? 12
For example:
A penetration tester might capture network traffic using tools like Wireshark. The OSI model helps
them dissect the data, layer by layer, to identify problems like unencrypted passwords Application
Layer issue) or incorrect routing Network Layer issue).
By understanding these models, penetration testers can better secure networks or find vulnerabilities to
exploit during tests.
Understanding the OSI Model in Simple Terms
The OSI Model Open Systems Interconnection) is a framework that explains how data travels between
two systems, step by step. It organizes the communication process into seven layers, each with a specific
job. Think of it as a relay race where each layer hands off the baton (data) to the next layer, ensuring the
message reaches its destination safely and reliably.
The 7 Layers of the OSI Model with Real-Life Examples
 Application Layer Layer 7
What it does Interfaces directly with the user or application. It handles the input and output of
data.
Example When you open a browser and type a URL, this layer handles your request. Protocols like
HTTP (web browsing) and SMTP (email) operate here.
Analogy Its like ordering a pizza through an app—this is where you interact with the service.
 Presentation Layer Layer 6
What it does Translates data into a format the application understands. It also handles encryption,
compression, and decryption.
Example SSL/TLS encrypting your web connection or converting images from .png to .jpg for
compatibility.
Analogy Think of this as the pizza kitchen preparing the food in a format everyone can eat (e.g.,
slices for sharing).
 Session Layer Layer 5
What it does Manages the session or connection between two systems, ensuring communication
remains active. It also handles reconnections if needed.
Example Keeping your login session alive on a website without needing to re-login repeatedly.
Analogy Its like reserving a table at a restaurant, ensuring you have a place to dine.
 Transport Layer Layer 4
What it does Ensures the data is delivered reliably and in order. It segments data streams and
manages congestion.
Example TCP (reliable delivery) or UDP (faster but less reliable delivery).
Analogy This is like packaging the pizza in a box to ensure it arrives intact.
 Network Layer Layer 3
What it does Routes data across networks, finding the best path to the destination using IP
addresses.
Example Routers use this layer to direct data to the right device using IPv4 or IPv6.
Analogy Its like the delivery driver using GPS to find your house.
What is Networking? 13
 Data Link Layer Layer 2
What it does Handles communication between devices on the same network and ensures errorfree transmission.
Example MAC addresses or switches directing traffic within a local network.
Analogy This is like ensuring the delivery driver uses the correct apartment buzzer code to enter
your building.
 Physical Layer Layer 1
What it does Transmits raw bits 0s and 1s) over cables, fiber optics, or Wi-Fi signals.
Example Ethernet cables, radio waves, or Bluetooth signals.
Analogy Its the physical road or path the delivery driver uses to bring your pizza.
The Layers at Work: Sending and Receiving Data
When you send data (e.g., visiting a website):
 The process starts at Layer 7 Application), where you type a URL.
 Each layer below adds its specific functionality (like routing, error checking, or encryption) until the
data is converted into electrical signals at Layer 1 Physical) and sent over the network.
When the data reaches the receiver:
 It travels in reverse, starting at Layer 1, where the physical signals are picked up.
 Each layer processes its part, removes unnecessary headers, and passes the data upward until it
reaches Layer 7, where its displayed as a readable webpage.
Real-Life Example: Sending a Text Message
Imagine sending a text message through a chat app:
 Application Layer Layer 7 You type and send the message.
 Presentation Layer Layer 6 The message is converted into a readable format for the recipient.
 Session Layer Layer 5 The app maintains a connection with the recipients app.
 Transport Layer Layer 4 The message is divided into small packets and sent reliably.
 Network Layer Layer 3 The packets are routed across the Internet to the recipient.
 Data Link Layer Layer 2 The packets are organized into frames for error-free transmission.
 Physical Layer Layer 1 The message travels as electrical signals or radio waves to the recipients
device.
The recipients device then unpacks and processes the message, reversing the layers, so they see it in
their chat window.
Key Points to Remember
Layers 14 Focus on reliable delivery (transport-oriented).
Layers 57 Focus on user interaction and applications (application-oriented).
Every layer performs specific tasks and uses the services of the layer below it.
Understanding this structure helps troubleshoot issues, analyze traffic, and secure communications,
which is why penetration testers and network engineers use it extensively.
What is Networking? 14
Understanding the TCP/IP Model in Simple Terms
The TCP/IP Model, also known as the Internet Protocol Suite, is a framework that explains how data
travels across the internet. It's simpler than the OSI model and has four layers, each focusing on a
specific task in the communication process. TCP/IP makes it possible for devices to communicate
regardless of the underlying hardware or network type.
The 4 Layers of the TCP/IP Model with Real-Life Examples
 Application Layer Layer 4
What it does Provides services and protocols that applications use to exchange data.
Example Protocols like HTTP (web browsing), FTP (file transfers), or SMTP (email).
Analogy Imagine placing a call to a customer service hotline—this is where you interact directly
with the service.
 Transport Layer Layer 3
What it does Manages the reliable delivery of data. It ensures that packets arrive correctly and in
the right order. It uses TCP for reliability and UDP for speed.
Example Streaming a video uses UDP (faster but less reliable), while downloading a file uses TCP
(ensures complete and error-free delivery).
Analogy This is like a delivery service ensuring your package arrives without damage, using
careful tracking or expedited methods depending on your needs.
 Internet Layer Layer 2
What it does Handles addressing and routing of data packets to ensure they reach the correct
destination. This layer uses IP Internet Protocol).
Example IP addresses guide data packets from your device to a website server and back.
Analogy Its like writing the destination address on a letter so the postal system knows where to
send it.
 Link Layer Layer 1
What it does Handles the physical connection between devices and places packets onto the
network medium. Its independent of the type of network (e.g., Ethernet, Wi-Fi, or fiber optics).
Example Ethernet cables or wireless signals transmit data between your router and your
computer.
Analogy Think of the road system that delivery trucks use to transport goods.
Key Tasks of the TCP/IP Model with Examples
 Logical Addressing IP
What it does Assigns unique addresses to devices to structure networks and route packets
correctly.
Example IPv4 (e.g., 192.168.0.1 or IPv6 (e.g., 20010db885a38a2e:03707334.
Analogy Its like assigning a street address to every house in a city to ensure mail is delivered to
the correct place.
 Routing IP
What it does Directs data packets through multiple nodes until they reach their destination.
What is Networking? 15
Example A router forwarding your request to access a website hosted on a server across the
globe.
Analogy Its like plotting the quickest route on a GPS from your house to a vacation spot.
 Error & Control Flow TCP
What it does Ensures data is sent and received correctly by maintaining a virtual connection and
sending control messages.
Example TCP resends a missing packet if it doesnt arrive or arrives corrupted.
Analogy Its like confirming over the phone that your friend received all the items you sent them.
 Application Support TCP
What it does Uses port numbers to differentiate between various applications on the same
device.
Example HTTP uses port 80, HTTPS uses port 443, and FTP uses port 21.
Analogy Think of each port as a different extension number in an office phone system.
 Name Resolution DNS
What it does Converts domain names (like www.google.com) into IP addresses (like
142.250.190.78.
Example DNS resolves the website name you type into your browser so your computer knows
where to send the request.
Analogy Its like using a phone book to find someones number based on their name.
TCP/IP in Action: Real-Life Data Transfer Example
 Application Layer Layer 4 You open a browser and request to visit a website (e.g., typing
www.example.com).
 Transport Layer Layer 3 Your device splits the website data into packets using TCP for reliable
delivery.
 Internet Layer Layer 2 The packets are routed across the internet using IP addresses, hopping
through routers.
 Link Layer Layer 1 The data is sent as electrical signals over Ethernet cables or Wi-Fi signals to the
next network device.
At the destination, the process works in reverse, rebuilding the data at each layer and delivering it to the
web browser as a complete webpage.
Comparing TCP/IP and OSI Models
Number of Layers OSI has seven layers; TCP/IP has four.
Focus OSI is a theoretical model for understanding communication; TCP/IP focuses on practical
implementation for internet communication.
Mapping The layers in TCP/IP combine some OSI layers (e.g., the Application Layer in TCP/IP
includes OSIs Application, Presentation, and Session layers).
Understanding both models is essential for troubleshooting, securing networks, and analyzing traffic,
especially in penetration testing or cybersecurity roles.
Understanding the Network Layer (Layer 3) in Simple Terms
What is Networking? 16
The Network Layer in the OSI model is like the traffic controller of a network. It ensures that data packets
find their way from the sender to the receiver, even if the two devices are in different networks or subnets.
This layer uses logical addressing (like IP addresses) and routing (finding the best path) to achieve this.
Key Functions of the Network Layer with Real-Life Examples
 Logical Addressing
What it does Assigns unique identifiers IP addresses) to devices in a network so packets know
where to go.
Example Your home has a street address (e.g., "123 Main Street"), and your computer has an IP
address (e.g., "192.168.1.10"). This address tells the network where to send data.
 Routing
What it does Finds the best path for data to travel from the sender to the receiver. It passes
through routers, which act like checkpoints or traffic lights on a highway.
Example Sending an email from the U.S. to Europe involves data packets traveling through
multiple routers across different networks before reaching the recipient.
Analogy Its like planning a road trip where you decide the best route to avoid traffic and reach
your destination efficiently.
Common Protocols in the Network Layer
These protocols are like sets of rules that define how data should be handled at this layer:
 IPv4 / IPv6
What they do Provide addressing and routing for packets. IPv6 is the newer version with longer
addresses for a growing internet.
Example IPv4 (e.g., "192.0.2.1") and IPv6 (e.g., "20010db88a2e:03707334") help routers and
devices understand where to send data.
 IPsec Internet Protocol Security)
What it does Secures data by encrypting and authenticating packets.
Example Used in VPNs to protect your internet traffic.
 ICMP Internet Control Message Protocol)
What it does Helps with troubleshooting by sending error messages (e.g., if a packet can't reach
its destination).
Example Ping uses ICMP to check if a device is reachable on the network.
 IGMP Internet Group Management Protocol)
What it does Manages group memberships for devices streaming the same content (like video or
audio).
Example Used for live streaming or multicast applications.
 RIP Routing Information Protocol)
What it does Shares routing information between routers to find the best path for data.
Example RIP tells routers the shortest path to send data packets to another network.
 OSPF Open Shortest Path First)
What it does Finds the fastest and most efficient path for data in large networks.
What is Networking? 17
Example OSPF is used in corporate networks to ensure data moves efficiently between
departments.
How the Network Layer Works
Sender Side:
The data packet is assigned a source IP address (the sender) and a destination IP address (the
receiver). The layer determines the best route for the packet.
During Transmission:
If the sender and receiver are in different networks, the packet is forwarded through multiple nodes
(routers). Each router reads the destination address, updates the routing path, and sends the packet
to the next node.
Receiver Side:
Once the packet reaches the destination network, the router forwards it to the device with the
matching IP address.
Real-Life Example
 You send a message to a friend in another country.
 The message (data packet) starts with your computer and gets routed through multiple routers across
the internet.
 Each router checks the destination IP address and forwards the packet closer to your friends device.
 Finally, the packet reaches your friend, who can read your message.
This process is seamless, thanks to the Network Layer efficiently managing addressing and routing.
IP Addresses: Simplified Explanation
In a network, every device (like a computer or smartphone) needs a unique identifier to communicate with
other devices. This is done using IP addresses, which work like digital addresses for devices in a network.
Understanding IP and MAC Addresses
 MAC Address
What it is A hardware-specific identifier (like a serial number) for network devices.
Purpose Used for communication within a single network (e.g., a home Wi-Fi network).
Analogy The MAC address is like an apartment number, specifying exactly where in a building a
person lives.
 IP Address
What it is A logical address assigned to a device for communication across networks, like the
internet.
Purpose Ensures data gets delivered to the right device, even if it's in a different network.
Analogy The IP address is like the postal address of the building.
IPv4: Structure and Format
IPv4 Internet Protocol Version 4 is the most common IP addressing system. Heres how it works:
Structure:
What is Networking? 18
IPv4 addresses are 32 bits long and divided into 4 groups called octets.
Each octet is represented as a number between 0 and 255, separated by dots (e.g., 192.168.10.39 ).
Example Representation:
Format Representation
Binary 1100 0000 . 1010 1000 . 0000 1010 . 0010 0111
Decimal 192.168.10.39
How Its CalculatedEach octet is a sum of powers of 2 for positions where the binary value is 1 .
Octet Binary Sum
1st 1100 0000 128 + 64 = 192
2nd 1010 1000 128 + 32 + 8 = 168
3rd 0000 1010 8 + 2 = 10
4th 0010 0111 32 + 4 + 2 + 1 = 39
Subnet Mask and CIDR
 Subnet Mask
What it is A number that defines which part of an IP address identifies the network and which
part identifies the device (host).
Example: 255.255.255.0 Binary: 11111111.11111111.11111111.00000000 ).
Octet Binary Decimal
1st 1111 1111 255
2nd 1111 1111 255
3rd 1111 1111 255
4th 0000 0000 0
How It Works:
The subnet mask indicates which bits in an IP address are for the network.
For 192.168.10.39 with subnet mask 255.255.255.0 , the network part is 192.168.10 , and the host
part is 39 .
 CIDR Classless Inter-Domain Routing)
What it is A compact way of writing an IP address with its subnet mask.
Example:
IP 192.168.10.39
Subnet Mask: 255.255.255.0
CIDR 192.168.10.39/24 ( /24 means the first 24 bits are for the network).
Classes of IPv4 Addresses
IPv4 addresses were traditionally divided into classes based on the range of addresses:
Class Range Subnet Mask CIDR Usable Hosts
A 1.0.0.0 - 127.255.255.255 255.0.0.0 /8 16,777,214
B 128.0.0.0 - 191.255.255.255 255.255.0.0 /16 65,534
What is Networking? 19
C 192.0.0.0 - 223.255.255.255 255.255.255.0 /24 254
D 224.0.0.0 - 239.255.255.255 Multicast Multicast Used for group messages
E 240.0.0.0 - 255.255.255.255 Reserved Reserved Reserved for research
Special Addresses
 Broadcast Address
What it does Sends a message to all devices in a network.
Example For network 192.168.10.0/24 , the broadcast address is 192.168.10.255 .
 Default Gateway
What it does Connects devices in one network to other networks (like the internet).
Example Typically the first or last usable IP in a network, e.g., 192.168.10.1 .
Binary and Decimal Conversion
 Binary to Decimal Add the values of all 1 bits in the binary form of an octet.
ExampleBinary: 11000000 Decimal: 128 + 64 = 192 .
 Decimal to Binary Subtract the highest power of 2 until reaching 0.
ExampleDecimal: 192 Binary: 11000000 .
Summary
IP addresses IPv4 are structured as four 8-bit groups called octets, separated by dots.
The Subnet Mask and CIDR notation help define the network and host parts of an IP address.
Classes A, B, and C are for general use, while D and E are for multicast and research purposes.
Understanding binary helps decode how IP addresses and subnet masks are represented and used.
Lets work through another example with subnetting to determine the Network Address, Broadcast
Address, First Host, Last Host, and the total number of Usable Hosts.
Example:
IPv4 Address: 10.0.1.35
Subnet Mask: 255.255.255.224
CIDR: /27
Step 1: Analyze the Subnet Mask
Subnet mask: 255.255.255.224
In binary: 11111111.11111111.11111111.11100000
The /27 indicates that 27 bits are reserved for the network part, leaving 5 bits for the host part.
Step 2: Calculate the Subnet Block Size
The block size is determined by the host bits 2^5 32.
So, 32 IP addresses are in each subnet.
Step 3: Find the Network Address
What is Networking? 20
The Network Address is obtained by setting all the host bits to 0.
 Convert the given IP 10.0.1.35 ) into binary: 00001010.00000000.00000001.00100011
 Apply the subnet mask ( /27 ): 00001010.00000000.00000001.00100000
 Convert back to decimal:Network Address: 10.0.1.32
Step 4: Find the Broadcast Address
The Broadcast Address is obtained by setting all the host bits to 1.
 Network bits remain unchanged: 00001010.00000000.00000001.00100000
 Set all host bits 5 bits) to 1 00001010.00000000.00000001.00111111
 Convert back to decimal:Broadcast Address: 10.0.1.63
Step 5: Calculate Usable Host Range
First usable host: Network Address 110.0.1.33
Last usable host: Broadcast Address 110.0.1.62
Step 6: Calculate Total Usable Hosts
Total IPs in the block: 2^5 = 32
Usable hosts: 32 - 2 (network + broadcast) = 30
Summary:
Parameter Value
Network Address 10.0.1.32
Broadcast Address 10.0.1.63
First Host 10.0.1.33
Last Host 10.0.1.62
Usable Hosts 30
Subnetting into Smaller Subnets:
Now lets divide this /27 into 4 subnets. Each subnet will have:
/29 prefix 27 2 bits).
Block size: 2^3 = 8 .
Usable hosts: 8 - 2 = 6 .
Subnet No. Network Address First Host Last Host Broadcast Address CIDR
1 10.0.1.32 10.0.1.33 10.0.1.38 10.0.1.39 10.0.1.32/29
2 10.0.1.40 10.0.1.41 10.0.1.46 10.0.1.47 10.0.1.40/29
3 10.0.1.48 10.0.1.49 10.0.1.54 10.0.1.55 10.0.1.48/29
4 10.0.1.56 10.0.1.57 10.0.1.62 10.0.1.63 10.0.1.56/29
