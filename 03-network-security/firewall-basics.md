# Firewall Basics

## Why This Topic
Understanding how firewalls work is essential for any cybersecurity analyst. Recruiters expect candidates to understand packet filtering, traffic flow, network segmentation, and basic rule structures. This document demonstrates my foundational knowledge of how firewalls operate and how they can be configured to protect an organisation.

---

## What Is a Firewall
A firewall is a security device or software that monitors, filters, and controls incoming and outgoing network traffic based on predefined rules. The goal is to prevent unauthorised access and allow legitimate communication.

---

## Types of Firewalls

### 1. Packet Filtering Firewall
- Evaluates packets based on headers such as IP address, port number, and protocol  
- Fast and lightweight  
- Limited visibility and cannot inspect payloads  

### 2. Stateful Firewall
- Tracks active connections  
- Only allows responses to legitimate traffic  
- More secure than packet filtering  

### 3. Proxy Firewall
- Works as an intermediary between internal systems and external servers  
- Masks internal IP addresses  
- Offers high security but introduces latency  

### 4. Next Generation Firewall (NGFW)
- Deep packet inspection  
- Application awareness  
- Integrated intrusion prevention capabilities  

---

## Common Firewall Rule Structure
Example using a simple conceptual format:

| Direction | Source IP | Destination IP | Protocol | Port | Action |
|----------|-----------|----------------|----------|------|--------|
| Inbound | Any | 10.0.0.20 | TCP | 443 | Allow |
| Outbound | 10.0.0.20 | Any | TCP | 80 | Allow |
| Inbound | Any | 10.0.0.20 | Any | Any | Deny |

Recruiters want to see that I understand:
- Allow rules  
- Deny rules  
- Priority order  
- Least privilege  

---

## Firewall Best Practices
- Deny by default and allow only what is required  
- Review rules regularly  
- Apply network segmentation  
- Log and monitor traffic  
- Use least privilege  
- Combine firewall rules with IDS or IPS visibility  

---

## Reflection
Learning firewall fundamentals allowed me to understand how traffic flows through a network and why correct rule configuration is essential. It also helped me appreciate the relationship between firewalls, IDS tools, and network segmentation. From a practical perspective, this knowledge prepares me to troubleshoot access issues, identify misconfigurations, and support secure network design in a real organisation.
