# Hybrid-Auction-PBS

Hybrid auction PBS
The purpose of this study is to investigate a hybrid auction format that does not alter the protocol and consensus and addresses user needs and expectations. We assume that protocols focus on the proposer's revenue, validity, trust assumptions, and market neutrality, while users focus on execution quality and inclusiveness.

We begin with a basic analysis of just-in-time (JIT) auctions, as represented by the current MEV boost, slot auctions that sell future slots, and hybrid auction models. The basic analysis includes auction definitions and information, risk, and capital requirements [1][2].

Hybrid auction formats will then be examined in the context of proposals related to PEPC-boost, Suave, and other partial block auctions, and the protocols and user implications in each format will be analyzed. The comparative analysis will then conclude the best auction format and implement it[3][4][5][6][7].

The final product will be published in the form of a research paper and blog post and implementation on Hybrid auction formats comparing PEPC-boost, Suave, and other partial block auctions in terms of protocols and user needs and expectations. (Only the auction format that was evaluated as the best within the study will be implemented.)

- 1.
  - 1.1 How much difference is there between Bid and Paylaod deadlines for JIT, Slot, and Hybrid?
  - 1.2 How do we define the latency for merging partial blocks in hybrid (partial block construction style)?
  - 1.3 How much of a disadvantage to Bid reduction or Proposer is caused by that latency?

- 2.
  - 2.1 How many preconf tips can be obtained through Slot Auction and Hybrid Auction preconfirmation?
  - 2.2 To what extent can preconf tips supplement the disadvantages（1.3） caused by the latency of merging partial blocks?
  - 2.3 If preconf tips do not cover it, how many seconds should we set the deadline for the payload?

- 3. 
  - 3.1 Hybrid Auction implementation in the context of the proposed partial block construction,
    - 3.1.1 ) How to design / implement Hybrid Auction
    - 3.1.2 ) Is it possible to design the Payload deadline to be at the time specified in 2.3?
    - 3.1.3 ) Which model, when compared, best fits the expectations and needs of the Protocol and users (e.g., if it increases the risk of timinge games, it is not secure for the Protocol)?
  - 3.2 Further issues and Future work

reference

- [1] https://mirror.xyz/0x03c29504CEcCa30B93FF5774183a1358D41fbeB1/CPYI91s98cp9zKFkanKs_qotYzw09kWvouaAa9GXBrQ
- [2] https://collective.flashbots.net/t/when-to-sell-your-blocks/
- [3] https://github.com/bharath-123/pepc-boost-docs/tree/main
- [4] [https://ethresear.ch/t/state-lock-auctions-towards-collaborative-block-building/
- [5] [https://research.eigenlayer.xyz/t/mev-boost-liveness-first-relay-design/
- [6] https://ethresear.ch/t/pepc-dvt-pepc-with-no-changes-to-the-consensus-protocol/
- [7] https://writings.flashbots.net/the-future-of-mev-is-suave
