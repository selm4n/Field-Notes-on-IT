# IP Addresses

Before talking about subnet masks, routing, or firewalls,
it helps to understand what an IP address actually is.

At its core, an IP address exists for one reason:
to identify where data should go.

---

## What an IP Address Really Does

When data moves across a network, the system needs an answer to a simple question:

Where should this data be delivered?

An IP address is that answer.

It does not describe the device.
It does not describe the user.
It only describes **location within a network**.

---

## The Structure of an IP Address

The most common IP format (IPv4) looks like this:

192.168.1.25

It is made up of four numbers separated by dots.
Each number represents a portion of the address.

At a high level, this address contains two parts:
- a **network** part
- a **host** part

Which part is which is not guessed.
It is defined using a subnet mask (covered later).

---

## Why IP Addresses Are Necessary

Without IP addresses:
- devices would not know where to send data
- networks could not scale
- routing would be impossible

Every packet sent across a network needs:
- a source IP (where it came from)
- a destination IP (where it should go)

No IP, no direction.

---

## IP Addresses Inside a Local Network

In home and office networks, devices usually receive private IP addresses such as:

192.168.1.10  
192.168.1.11  
192.168.1.12  

These addresses are only meaningful inside that local network.
They are not visible on the public internet.

A router sits between the local network and the outside world
and handles communication beyond it.

---

## IP Addresses on the Internet

From the internet’s point of view,
a network usually appears as a **single IP address**.

Internally, many devices may exist,
but externally they are represented by one public address.

This separation between internal and external addressing
is a key concept in networking and security.

---

## What an IP Address Is Not

An IP address:
- is not a username
- is not a password
- does not grant access by itself

It is simply an address.
Access control is handled by other systems.

---

## One-Line Takeaway

An IP address exists to tell a network where data should be delivered.
