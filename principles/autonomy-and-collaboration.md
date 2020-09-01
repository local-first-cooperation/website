---
layout: default
---

# Design for Autonomy and Collaboration

The ultimate goal of Edge Native is to obtain a system that is maximally useful, even under adverse conditions. As long as one edge device is functioning, the apps on it shall be usable: while new information from other devices cannot be received, the user can still view the stored data and register new information or interact with locally modelled workflows. As soon as a second functioning edge device comes into communication range, information can flow between them and allow inter-device workflows to be used, for example for the collaboration between their users.

This is achieved by designing an Edge Native application to assert its own autonomy, claim ownership of its local data, and function independently of everything else. This is to say that the collaboration with other edge devices must not be required for useful function, but of course it lies in the nature of some application functions that they are less useful while there are no communication partners.

On the other hand, Edge Native applications are ultimately built for collaboration, they are not expected to be used without communication partners indefinitely. Therefore, such an application is coded with a focus on how information will be exchanged with other devices, collaboration is baked into it.

An Edge Native application is capable of but not constantly tied to communication.