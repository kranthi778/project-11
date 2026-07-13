# Project 11. Denial of Service (DoS) Attacks

# Part 1 – Introduction to Denial of Service (DoS)

## Objective

I want to understand the basics of Denial of Service (DoS) and Distributed Denial of Service (DDoS) attacks. I need to know how they affect system and network availability and what techniques attackers use.

# What is Denial of Service (DoS)?

A Denial of Service (DoS) attack is when someone tries to make a computer, server, application or network resource to its users. This happens by using up its resources like CPU, memory, bandwidth or network connections.

The main goal of a DoS attack is to stop a service from working not to steal data like in types of attacks.

# What is Distributed Denial of Service (DDoS)?

A Distributed Denial of Service (DDoS) attack is a version of a DoS attack. Here many infected devices work together to send a lot of traffic to one target.

These infected devices are called bots or zombies. Someone controls them from a distance.

# DoS vs DDoS

Here's a comparison:

* Denial of Service (DoS) uses one attacking system.

* Distributed Denial of Service (DDoS) uses infected systems.

* DoS is easier to detect.

* DDoS is harder to detect.

* DoS sends traffic.

* DDoS sends traffic.

* DoS is easier to stop.

* DDoS is harder to stop.

![Alt text](screenshots/dos-vs-ddos-comparison.png)

**DoS vs DDoS**

```text

dos-vs-ddos-comparison.png

```

# Botnet

A botnet is a group of devices connected to the Internet that are infected with malware. Someone controls them from a distance.

Botnets are often used for:

- DDoS attacks

- Sending spam emails

- Spreading malware

- Creating Internet traffic

![Alt text](screenshots/botnet-overview.png)

**Botnet**

```text

botnet-overview.png

```

# Common DoS Attack Types

Some common Denial of Service attack techniques are:

- TCP SYN Flood

- UDP Flood

- HTTP Flood

- Ping of Death

- MAC Flooding

Each of these attacks targets different protocols or network resources to overwhelm the target system. This prevents users from accessing services.

# Countermeasures

To reduce the impact of DoS and DDoS attacks organizations can use:

- Firewalls

- Intrusion Detection Systems (IDS)

- Intrusion Prevention Systems (IPS)

- Traffic Filtering

- Rate Limiting

- Load Balancers

- Web Application Firewalls (WAF)

- Content Delivery Networks (CDN)

- Continuous Network Monitoring

![Alt text](screenshots/dos-countermeasures.png)

**Countermeasures**

```text

dos-countermeasures.png

```

# Learning Outcome

After learning this I now know:

- The difference between DoS and DDoS attacks.

- How botnets are used for DDoS attacks.

- Common types of DoS attacks.

- measures to reduce DoS attacks.

- Why service availability is important, during cyberattacks.

# conclusion

In this part I learned about Denial of Service (DoS) and Distributed Denial of Service (DDoS) attacks. 
I now understand how botnets contribute to large-scale attacks, techniques used to disrupt services and defensive measures to maintain system availability.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Project 11. Denial of Service Attacks

# Part 2 – Common Denial of Service Attack Techniques

## Objective

I want to understand the Denial of Service attack techniques that are used the most. I need to know how these Denial of Service attacks target network resources and how they affect system availability.

---

# TCP SYN Flood

A TCP SYN Flood attack is when someone sends a lot of SYN requests to a server without finishing the connection. This is like a handshake. When you shake hands with someone you expect them to shake back.. In this case the person just keeps putting out their hand without waiting for a response.

As a result the server gets tired of waiting and runs out of resources. This means that real users cannot connect to the server. The Denial of Service attack is successful because the server is busy waiting for all these connections to finish.

### Characteristics

- The TCP SYN Flood attack uses the three-way handshake.

- It creates a lot of half open connections.

- It uses up the servers memory and connection resources.

- It makes the service less available to users.

![Alt text](screenshots/tcp-syn-flood-overview.png)

![Alt text](screenshots/tcp-syn-flood-overview2.png)
**TCP SYN Flood**

```text

tcp-syn-flood-overview.png

```

I need to get the **TCP SYN Flood** diagram from the CEHv13 module.

---

# UDP Flood

A UDP Flood attack is when someone sends a lot of UDP packets to a server. The server tries to process each packet. It gets overwhelmed. This is like trying to drink from a firehose. The server just cannot keep up.

The UDP Flood attack uses the UDP protocol to send packets to specific ports on the server. The server tries to process each packet. It uses up a lot of bandwidth and processing power.

### Characteristics

- The UDP Flood attack uses the UDP protocol.

- It uses up a lot of bandwidth.

- It makes the server work harder which increases CPU utilization.

- It might also generate ICMP responses.

---

# ICMP Flood

An ICMP Flood attack is when someone sends a lot of ICMP Echo Request packets to a server. This is like an echo. The server keeps responding to each request but it gets overwhelmed.

This type of Denial of Service attack is also known as a Ping Flood. The ICMP Flood attack sends ICMP Echo Request packets to overwhelm the target system or network.

### Characteristics

- The ICMP Flood attack uses ICMP Echo Requests.

- It uses up a lot of bandwidth.

- It makes the network slower, which increases latency.

- It might make some services unavailable.

---

# HTTP Flood

An HTTP Flood attack targets web applications by sending a lot of HTTP requests. These requests look real. It is hard to tell them apart from legitimate traffic.

The HTTP Flood attack is different from floods because it works at the application layer. This means it targets web servers specifically.

### Characteristics

- The HTTP Flood attack targets web servers.

- It is hard to distinguish from traffic.

- It uses up web server resources.

---

# Other Flooding Attacks

There are types of flooding attacks, such as the Ping of Death MAC Flooding and Smurf Attack. Each of these Denial of Service attacks uses a technique but they all have the same goal. To use up system or network resources and deny service to real users.

---

# SOC Analyst Perspective

SOC analysts watch network traffic to find spikes excessive SYN packets, abnormal UDP traffic, ICMP floods and a lot of HTTP requests. If they find something they can investigate and take action before the services become unavailable. This is, like having a security guard who watches the network and protects it from Denial of Service attacks.

---

# Key Concepts Learned

- TCP SYN Flood

- UDP Flood

- ICMP Flood

- HTTP Flood

- Ping of Death

- MAC Flooding

- Smurf Attack

- Network Availability

---

# conclusion

In this part I learned about the most common Denial of Service attack techniques. I learned how these Denial of Service attacks target network protocols to use up system resources. 
I also learned how security teams find these attacks and protect network availability by watching the network and using controls. 
The Denial of Service attacks are a threat but with the right knowledge and tools we can protect our networks and systems.
