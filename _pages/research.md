---
permalink: /research/
title: "Research"
author_profile: true
---

Active Channel Sparsification for FDD Massive MIMO
------
Realizing a massive MIMO system in frequency division duplexing (FDD) mode is known to be challenging due to the high channel training and feedback overhead: in such systems Uplink/Downlink channel reciprocity does not hold, and in order to obtain Downlink CSI the base station needs to (a) transmit pilots to the users, (b) receive the pilot measurements from the users via Uplink closed-loop feedback, and (c) estimate the Downlink channel of each user from its corresponding feedback. A conventional estimator would require $T\ge M$ pilots to perform this task (where $M$ denotes the channel dimension), but the problem is that with a massive array consisting of $M\gg 1$ antennas, spending such a large number of Downlink pilots essentially results in exhausting the time-frequency resources, leaving little to no resources for data transmission.

Given a fixed (limited) pilot dimension $T<M$, the idea behind <em>active channel sparsification</em> (ACS) is to estimate the <em>effective</em> CSI in a smart way such that the multi-user channel matrix rank, equivalent to the Downlink multiplexing gain, is maximized. This involves designing a precoding matrix that, once concatenated with the channel, reduces its number of independent coordinates to less than the available pilot dimension, enabling a stable estimate of the effective channel. The idea is implemented by forming a user-virtual beam bipartite graph model and maximizing the graph maximal matching size by solving a mixed integer linear program. The outcome is a novel precoding scheme with significant achievable sum-rates with any given pilot dimension (perhaps specified by the protocol) for various FDD massive MIMO communication scenarios.

Our paper on ACS can be found [here](https://ieeexplore.ieee.org/abstract/document/8542957).

<img src="{{https://mbarzegar.github.io}}/images/bipartite.png" style="display: block; margin: auto;" />