---
layout: default
---

# Edge Native from First Principles

## Prelude: A Tale of Two Robots

Imagine a universe that is empty bar two robots and a box. The robots are called Marvin — who is holding the box — and Maximilian. Marvin wants to hand off the box to concentrate fully on his gloomy thoughts. The only means by which Marvin can learn of a possibility to shed the box is by one of the four fundamental forces of physics. The so-called *weak* and *strong* interactions have extremely short range (only a quadrillionth of a meter), *gravity* is barely detectable between these robots and extremely hard to harness for sending and detecting signals, leaving *electromagnetic radiation* as the logical choice. Marvin could send radio waves or light, for example, and detect the response of Maximilian’s body to these probes.

At this point, a nested thought experiment is in order: if we could place anything else into that universe, could we make it easier for Marvin to find out about Maximilian? The answer is no. Whatever we placed, Marvin would have to find out about it before he could make use of it, which brings us back to square one. And even if this was not the case — i.e. assuming that Marvin “just knows” about the thing — the interaction between Marvin and the new thing will have to be more complex, as merely knowing of the presence of another thing cannot reveal the existence of Maximilian; Marvin will have to communicate, which implies a dependency on the other thing to respond. This makes it impossible for Marvin to fully own the discovery process, to drive every step of it, to ascertain that it works as long as he — Marvin — continues to function. The added dependency introduces a new source of failure. What a delectable misery, Marvin would think.

Now that Marvin knows of Maximilian’s existence, he must ask him to rid him of the box. Again, the logical choice for this endeavour is to send signals via electromagnetic radiation, hoping that Maximilian is capable of receiving them and of responding in kind. If all goes well, both robots can thus coordinate their approach and the hand-over of the box, and Maximilian even suppresses his urge to destroy Marvin’s circuits (yes, Maximilian is a *bad robot*).

Here, we perform a similar nested thought experiment: if the universe were any less empty, could this help with the communication? As long as the two robots speak the same language and use the same radio frequencies and modulation, the answer is again a firm “no”. Any other thing would have to act as an intermediary, adding to the amount of communication paths that need to function and to the number of messages that need to be sent in total (which also increases the time needed for coming to an agreement, which may be important to Marvin). The success of the exchange then depends not only on Marvin and Maximilian but also on the other thing’s ability to perform its signal-forwarding duties. Only in the case where Marvin and Maximilian do not share a common message transport (like one having only an S-band antenna and the other an L-band, or Marvin insisting on the most pessimistic BPSK while Maximilian will only speak 1024QAM with OFDMA) is it helpful — even necessary — to add a suitable translator.

## Abstraction: Core Tenet of Edge Native

The situation between Marvin and Maximilian (except for the latter’s sinister desires) applies to many situations in the world as humankind knows it, all we need to do is to define a suitable mapping — in other words, we can find the two robots embedded in the world around us and reduce the situation to their essential dilemma by removing everything else from consideration.

Take for example an autonomous mobile logistics robot as it approaches a mobile production cell for a car with the soon needed door. The logistics robot will orient itself correctly towards the active beacons of the production cell and coordinate the hand-over of the door directly with the robot arms installing the door on the car frame. Everything else in the universe (short of emergency shutdown switches) is completely irrelevant, we can imagine that Marvin the logistics robot hands the box (door) to Maximilian the production cell.

Or a Mars rover returns to its base station to recharge and perform a full data dump; a hotel guest’s mobile phone at the reception desk receives the cryptographic material to unlock a room door for the next 72 hours; a car asking the roadside beacons for current surface conditions or high-resolution map data. Note how in all these situations the addition of intermediaries only makes matters worse: it increases latency and diminishes reliability. The most dependable fashion of implementing these scenarios is by direct communication between local interlocutors.

> This is the core tenet of Edge Native computing: local participants communicating directly with one another.

Intermediaries are needed for translation services, which is meant not only in the linguistic sense but also in the geometrical: when the information is available in one location but needed in another and the respective devices do not have sufficient reach for direct communication, message forwarders can enable the flow of information — the information is *translated* along the cartesian coordinates. This is also relevant in the fourth dimension, where the information is stored by a stationary device in one location so that it can be acquired by another device at a later time.

> The core tenet is thus enlarged to cover collaborating groups of devices where necessary to bridge larger distances in space or time.

A few consequences directly follow from the above:

- A participant can only communicate what it knows.
- Communication takes time (speed of light, plus available bandwidth), so transferred information always pertains to the past — it may be a plan for the future, but made some time ago.
- The recipient will need to decide whether to trust the received information, where a strong concept of identity comes in handy.
- Mobility of participants implies the need for relaying information, e.g. to make it available in the same physical location at a later time.

## Protocol: Core Principle of Edge Native

We started from the premise of the dynamic emergence of communication relationships. While some conversations including the nature and identity of all interlocutors can be foreseen (and thus statically programmed), our world will be less brittle, richer, and more fun by allowing it to be more dynamic. When Marvin meets Maximilian, he initially knows nothing about his new acquaintance; similarly, Maximilian will need to judge the situation to incorporate the presence of Marvin and map out possible plans of action. It would be an undesirable restriction to demand that whoever programmed Marvin also knew how Maximilian worked and vice versa. It would be equally stifling to fix the permissible workings of a robot ahead of time.

The solution to this problem is that the communication protocol makes as little assumption as possible about how the recipient will make use of the transferred information. The value that can be extracted from a conversation is therefore maximised by sending facts instead of their local interpretation. In the example, Marvin should tell Maximilian about the dimensions and weight distribution of the box; if he told him instead where to grip it then these instructions were likely suboptimal because Marvin cannot know the precise mechanics of Maximilian’s gripping system — nor should he.

> Edge Native systems transfer and persist facts, not interpretation.

In addition to the characteristics of the box Marvin will communicate that he wants to get rid of it. This serves to demonstrate that the decisions made by autonomous edge devices are also facts that are worthy of dissemination, because Maximilian will need the information to make a decision for himself.

## Philosophy: Accept Uncertainty when Making Decisions


