---
layout: default
title: Edge Native
---

# What is Edge Native?

*Edge Native* means *born and raised on the edge*, more precisely the edge of the global web of computer networks.
The Internet started out promising *end-to-end connectivity* between computers on all continents, allowing collaboration on a global scale.
Edge Native brings ubiquitous networking down to the smallest scale:
local collaboration between computers — edge devices — on tasks that do not require global resources.

> Edge Native applications fulfill their function using local resources, communicating with local peers, without requiring synchronous access to remote resources.

In particular, an Edge Native application running on an edge device may communicate with a [Cloud Native](https://www.cncf.io/) application to enable global workflows and information flow.
But the mission critical paths of the Edge Native application do not depend on momentarily being able to reach that Cloud Native application.
Edge Native applications practice the [local-first imperative](https://www.inkandswitch.com/local-first.html) while explicitly aiming for local collaboration with other devices.
This collaboration is performed directly, without intermediaries and with as little infrastructure as possible; most importantly it is not performed via the cloud.

# Edge Native Principles

- [communicate locally](principles/communicate-locally.html)
- [design for autonomy and collaboration](principles/autonomy-and-collaboration.html)
- [communicate facts, not interpretation](principles/communicate-facts.html)
- [accept uncertainty when making decisions](principles/accept-uncertainty.html)
- [design the flow of information](principles/information-flow.html)
- [employ scoped consistency only where required](principles/scoped-consensus.html)
- [decouple computation in space and time](principles/decouple-space-time.html)

The above are [derived from first principles](first-principles.html).

# Relationship with the Reactive Manifesto

The above principles have a remarkable overlap with the principles derived from the [Reactive Manifesto](https://reactivemanifesto.org).
This is not a coincidence: the desire to stay responsive on a single edge device shares a lot with ensuring that a cloud service stays responsive, even though the underlying infrastructure faces different challenges in detail.
The confluence between Reactive principles for Edge Native and Cloud Native applications is elaborated in [this article](reactive-edge-native.html).
