---
layout: default
title: Local-First Cooperation
---

# Executive Summary

Humankind is the most resilient higher life form on this planet, which stems from two main characteristics: highly adaptive and tenacious individuals plus the capability of complex and abstract cooperation.
Our usage of computers has added to our capabilities but has also made us more vulnerable by centralisation, creating single points of failure.
We need to mirror our natural resilience in our computer designs to take the next step forward, otherwise we will fail.
This resilience needs to be woven into the fabric of all our digital interactions, from manufacturing of goods over healthcare, economic services, and public authority to social networks.

We call this design goal **local-first cooperation** and derive some core principles on which such software systems are built:

- require only **local communication** for local interactions — going via a central message exchange always adds potential for failure
- **each part acts autonomously**, with decisions being taken on the local computing device
- construct the parts for **cooperation between them**, solve larger problems using multiple devices working together
- **communicate facts**, not interpretation, to allow other parts to make their own decisions
- **accept uncertainty** and make decisions based on local but possibly incomplete information
- expect **dynamic changes** in the network of neighbouring and collaborating parts

Upon this basis we can build more complex interactions, forming hierarchical behaviour and covering longer distances in space and time, but we must not violate the above core principles while doing so.
From the principles follow some further restrictions, most notably that we can only employ consensus (i.e. have a strongly consistent data model) when we can afford the latency and fallibility that come with it.
The principles also give guidance in terms of software architecture, namely that data structures need to support evolution over time since we store facts, and that the flow of information is a primary design target.

## The Plan

Our plan is to create and refine software tools that make it simple and easy to build resilient software according to the principles outlined above.
We aim for a multitude of tools to grow that each cover some particular part of the problem or an application domain.
By adhering to the above principles, the software that will be built on these tools will be able to cooperate on a much larger scale, between different implementations.
Out of this experience may eventually emerge a set of communication standards, but we deliberately do not start from that end — we let nature run its course to find the optimal solution.

## Get Involved

The endeavour outlined above is far greater than any single person or organisation who contributes.
If you want to help push this forward you are very welcome to join us:

- ask to join our [email group](https://groups.google.com/g/local-first-cooperation) (your address will only be visible to group admins)
- review more material on this website and contribute to it [on github](https://github.com/local-first-cooperation/website)
- spread the word by forwarding this information to those who you think should contribute

---

# Robust cooperation between nearby computing devices

_Since about a decade we are seeing tremendous growth in the capabilities of mobile computing devices.
At the same time we are outfitting more and more things with computing capabilities and connecting them to the Internet.
Besides the undoubtedly useful global connectivity and the countless services that are provided thanks to it, we believe it is time to start making use of the information technology that we hold in our hands and that exists around us.
We need to start using **local computing resources** to their full capability and employ IT for **cooperation between neighbours**._

This document does not yet have a final name itself and is related to a few other concepts:

- [local-first](https://www.inkandswitch.com/local-first.html)
- “(mobile) edge device native” as opposed to (and complementary to) [cloud native](https://www.cncf.io/)
- “edge computing”, which so far unfortunately sees local computation only as pre-processor for the cloud, not independently

After some introductory remarks, we formulate [principles](#local-first-cooperation-principles) that must underlie all collaborative software that stays maximally useful under all operating conditions.
These principles are derived from the idea that it should be enough for two computing devices to be connected to each other for them to cooperate, and to facilitate cooperation of their respective users.

These principles have a remarkable overlap with the [reactive principles](https://principles.reactive.foundation/) derived from the [Reactive Manifesto](https://reactivemanifesto.org).
This is not a coincidence:
the desire to stay responsive on a single edge device shares a lot with ensuring that a cloud service stays responsive, even though the underlying infrastructure faces different challenges in detail.
The confluence between local-first and reactive principles is elaborated in [this article](reactive-edge-native.html).

## Why this is important

One example is **industrial manufacturing:** we as humankind owe our invaluable advancements in living standard, common wealth, and medical abilities to the efficient and repeatable production of goods of all kinds, be that food, furniture, clothing, or medicine.
We can make industrial production even more efficient, less wasteful, and thus create more common wealth and human advancement by enlisting the help of IT on the factory shop-floor.
But for that to be successful, these IT systems need to be as reliable as the paper-based processes that they replace.
And they need to retain the distributed and resilient nature of our production plants — we must not make this backbone of our civilisation more brittle by centralising its decision-making processes.

Another example is **cooperation between humans:**
The cloud has enabled collaborative software that lets people from all over the world work together on shared documents, fuelling our creativity.
But it has also taken away agency and ownership of our data; when using these services we borrow our own data from a service provider who may cease to exist.
In order to preserve and archive those creative works we need to retain them on our own local devices.
And we want to be able to collaborate without the constraint of having a central cloud service available and reachable:
as long as two capable devices are connected, we want to allow their human users to benefit from their collaborative capabilities.

Other examples include swarm intelligence within a **fleet of autonomous vehicles**, or the daily interactions between people and **services or goods we buy**.
While there are some parts that are enabled by cloud computing, would it not be awesome to have the essential part — the local interaction — work independently of any centralised processing?
This way, what must always work will work as long as two things are nearby and ready to interact.
And in this way, we can give everyone control over their data, to be shared willingly where needed.

## Who should read this

This document should be read by everyone who creates IT applications through which humans and/or machines interact with one another.
Too much software today fails in unintuitive ways when cloud services are unavailable or slow to reach.
Even if you don’t agree with the goals, the below principles explain why not adhering to them creates software that is less robust and less useful than it could be.

## What you can do

This document is still in its infancy and needs to grow up.
If you want to help push this forward you are very welcome to join us:

- ask to join our [email group](https://groups.google.com/g/local-first-cooperation) (your address will only be visible to group admins)
- review more material on this website and contribute to it [on github](https://github.com/local-first-cooperation/website)
- spread the word by forwarding this information to those who you think should contribute

# Local-First Cooperation Principles

The following principles give rise to IT systems that stay maximally useful to their local end-users under all conditions:

- [communicate locally](principles/communicate-locally.html)
- [build autonomous parts](principles/autonomy.html)
- [design parts for cooperation](principles/cooperation.html)
- [communicate facts, not interpretation](principles/communicate-facts.html)
- [accept uncertainty when making decisions](principles/accept-uncertainty.html)
- [foresee dynamic changes in the network neighbourhood](principles/foresee-network-dynamics.html)

These principles are [derived from first principles](first-principles.html).
Adhering to the above principles implies some further constraints on software design:

- [hierarchical systems to cover space and time](principles/hierarchical-systems.html)
- [employ scoped consistency only where required](principles/scoped-consensus.html)
- [design the flow of information](principles/information-flow.html)


