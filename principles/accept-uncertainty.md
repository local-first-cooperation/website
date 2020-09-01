---
layout: default
---

# Accept Uncertainty when Making Decisions

Next to the observation of environmental facts there is another important source of facts that Edge Native applications react to: decisions taken by end-users or algorithms. The decision to perform a workflow step, to take on a logistics mission, or to send a chat message is an important fact that is created locally, possibly affecting other edge devices elsewhere.

The most conspicuous difference between Edge Native applications and traditional applications built around transactional databases is that an autonomous edge device cannot hope to have access to a complete picture of the whole system, its state is always incomplete, missing facts from other edge devices that have not yet been received. The strictly serialised transactional database on the other hand allows the application programmer to act with godlike overview, as if Laplace’s demon could also make changes to the world. Because the latter superpower is bought at the price of introducing a well-known fallible *single point of failure*, Edge Native applications must instead confidently make decisions based on incomplete information.

Consequently, these decisions will sometimes turn out to have been incorrect, for example by noticing that two robots took the same mission and are now duplicating the effort. The application recognises this mistake by observing the facts emitted by the other edge devices and will then take measures to correct it — in other words, asking for forgiveness instead of being blocked waiting for permission.