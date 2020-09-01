---
layout: default
---

# Employ Scoped Consensus only Where Required

Creating consensus between computers is the act of asking a group of computers to take a decision — for example on what the next database transaction shall be — and using an algorithm between them that ensures that all computers come to the same decision (modulo those that fail in the process). From this description it is obvious that waiting for such a group decision breaks the autonomy of a single edge device (not to mention the FLP result that proves that it is impossible to create a consensus algorithm that successfully concludes under all circumstances).

There are use-cases, though, that require consensus: consider having two rockets on Mars capable of intercepting and destroying an incoming meteorite and an algorithm that needs to launch exactly one of those when armageddon looms (because the other rocket will be needed soon thereafter). Or, in less dramatic terms, sending an invoice just once for the goods that just left the factory because customer service is everything.

When consensus is needed in an Edge Native application, it is established only between those edge devices that need to agree on a single outcome, and only for those decisions that require it. The result is then communicated as facts so that applications elsewhere may react to it in a fully autonomous fashion again, without spreading the need for consensus throughout the whole system.