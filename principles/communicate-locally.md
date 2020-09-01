---
layout: default
---

# Communicate Locally

An Edge Native application communicates locally with its neighbouring edge devices, with as little dependency on infrastructure as possible. This can be done in many ways, including ethernet, field buses, wifi, bluetooth, UWB, etc. While each single edge device may fail, the failure of one part of the system never hinders the remaining parts from collaborating. Formulated the other way around, the communication and collaboration of two edge devices does not crucially depend on a single other device. This makes the system as a whole as resilient to failure as possible — another way of looking at this is that sabotaging the system requires disabling many edge devices, there is no central point that can be attacked.

The above definition may seem very restrictive, but it allows large and complex networks and processes to be formed. Where the range of a communication transport does not have sufficient reach to connect two collaborating edge devices, others can forward the messages to help out. This is permitted if there always is redundancy in the mesh network, so that in the case where a forwarding device fails other routes via different forwarders will automatically be taken.

Where two edge devices communicate directly with one another, message transmission latency can be strictly bounded to allow real-time interaction. Forwarding the messages via other edge devices does not only introduce additional latency, it also leads to momentarily increased latency while new routes are found following a failure in the forwarder chain. This effect can be mitigated at the cost of higher bandwidth requirements by always forwarding messages via multiple independent routes.