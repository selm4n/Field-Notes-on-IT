# Subnet Masks

Subnet masks are one of those topics that sound more complex than they are.

At first, they feel abstract.
But once the purpose is clear,
everything else starts to make sense.

---

## Why Subnet Masks Exist

An IP address by itself is not enough.

When a system sees an IP address,
it still needs to answer one question:

Which part of this address refers to the network,
and which part refers to the specific device?

That separation is what a subnet mask defines.

---

## What a Subnet Mask Does

A subnet mask tells the system how to interpret an IP address.

It does not change the IP.
It does not assign addresses.
It only **draws a boundary**.

On one side of that boundary:
- the network portion

On the other side:
- the host portion

Without this boundary,
the system would not know
which devices are considered “local”.

---

## A Common Example

IP address:

192.168.1.25

Subnet mask:

255.255.255.0

This combination tells the system:

- the first three numbers identify the network
- the last number identifies the device

In practice, this means:
any device with `192.168.1.x`
is considered part of the same local network.

---

## Why This Matters

When a device wants to send data,
it first checks:

Is the destination in my local network?

The subnet mask is used to answer that question.

- If the destination is local, send directly
- If not, send the traffic to a router

This decision happens constantly
and automatically.

---

## What Happens Without a Subnet Mask

Without a subnet mask:
- every destination would look ambiguous
- local and remote traffic could not be separated
- routing would break down

Subnet masks make efficient communication possible.

---

## Subnet Masks Are Not About Security

A common misconception is that subnet masks
are a security feature.

They are not.

Subnet masks are about **organization and routing**.
Security is handled by other mechanisms,
such as firewalls and access controls.

---

## A Practical Way to Think About It

An IP address tells you *where* something is.
A subnet mask tells you *how much of that location matters locally*.

Together, they allow systems
to communicate efficiently
without confusion.

---

## One-Line Takeaway

A subnet mask defines which part of an IP address belongs to the network and which part belongs to the device.
