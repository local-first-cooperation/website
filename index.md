---
layout: default
title: Swarm Computing
---

# Robust collaboration between nearby computing devices

_Since about a decade we are seeing tremendous growth in the capabilities of mobile computing devices.
At the same time we are outfitting more and more things with computing capabilities and connecting them to the Internet.
Besides the undoubtedly useful global connectivity and the countless services that are provided thanks to it, we believe it is time to start making use of the information technology that we hold in our hands and that exists around us.
We need to start using **local computing resources** to their full capability and employ IT for **collaboration between neighbours**._

This document does not yet have a clear name itself and is related to a few other concepts:

- [local-first](https://www.inkandswitch.com/local-first.html)
- “(mobile) edge device native” as opposed (and complementary) to [cloud native](https://www.cncf.io/)
- “edge computing”, which unfortunately sees local computation only as pre-processor for the cloud, not independently

## Why this is important

One example is **industrial manufacturing:** we as humankind owe our invaluable advancements in living standard, common wealth, and medical abilities to the efficient and repeatable production of goods of all kinds, be that food, furniture, clothing, or medicine.
We can make industrial production even more efficient, less wasteful, and thus create more common wealth and human advancement by enlisting the help of IT on the factory shop-floor.
But for that to be successful, these IT systems need to be as reliable as the paper-based processes that they replace.
And they need to retain the distributed and resilient nature of our production plants — we must not make this backbone of our civilisation more brittle by centralising its decision-making processes.

Another example is **collaboration between humans:** _TODO (Martin?), also link to local-first_

Other examples include swarm intelligence within a **fleet of autonomous vehicles**, or the daily interactions between people and **services or goods we buy**.
While there are some parts that are enabled by cloud computing, would it not be awesome to have the essential part — the local interaction — work independently of any centralised processing?
This way, what must always work will work as long as two things are nearby and ready to interact.
And in this way, we can give everyone control over their data, to be shared willingly where needed.

## Who should read this

This document should be read by anyone who creates IT applications through which humans and/or machines interact.
Even if you don’t agree with the goals, the below principles explain why not adhering to them creates software that is less robust and less useful than it could be.

## What you can do

This document is still in its infancy and needs to grow up.
It would be most helpful if you could head over to [github](https://github.com/edge-native/website/) and suggest improvements or note shortcomings.
We appreciate all inputs!

# Swarm Computing Principles

The following principles give rise to IT systems that stay maximally useful to their local end-users under all conditions:

- [communicate locally](principles/communicate-locally.html)
- [design for autonomy and collaboration](principles/autonomy-and-collaboration.html)
- [communicate facts, not interpretation](principles/communicate-facts.html)
- [accept uncertainty when making decisions](principles/accept-uncertainty.html)
- [design the flow of information](principles/information-flow.html)
- [employ scoped consistency only where required](principles/scoped-consensus.html)
- [decouple computation in space and time](principles/decouple-space-time.html)
- [foresee dynamic changes in the network neighbourhood](principles/foresee-network-dynamics.html)

The above are [derived from first principles](first-principles.html).

## Relationship with the Reactive Manifesto

The above principles have a remarkable overlap with the [principles](https://principles.reactive.foundation/) derived from the [Reactive Manifesto](https://reactivemanifesto.org).
This is not a coincidence: the desire to stay responsive on a single edge device shares a lot with ensuring that a cloud service stays responsive, even though the underlying infrastructure faces different challenges in detail.
The confluence between Reactive principles for Edge Native and Cloud Native applications is elaborated in [this article](reactive-edge-native.html).
