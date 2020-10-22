# Community Mana what ifs...


* If this is correct (https://thetangle.org/statistics/tokens-distribution) about 0.07% of addresses hold ~70% of all tokens. This means that even if 99.93% of addresses contribute towards active, honest mana, that's only ~30% of total mana.  How 0.07% of addresses controlling 70% of tokens is not a problem at all (for consensus, or voting, or data throughput, etc) (given the token )

* It seems that saturating the network would be beneficial to those holding lots of Mana (assuming they are able to sell or lend their Mana). What's the percentage of (active/passive) Mana held by honest node owners required to prevent artificial network saturation in order to prevent the emergence of a market of fee-based transactions, assuming that malicious node owners might saturate the network artificially ("spam") in order to be able to sell their network capacity (or Mana) (to the highest bidder).

* Is it possible to approve double spends by approving two conflicting transactions and embedding them into the tangle if there are enough malicious node owners "approving" them? What's the percentage of (active/passive) Mana that would be required to successfully do this? How would honest nodes react to relayed, yet conflicting transactions a majority of malicious node owners/Mana holders has voted to be legitimate

* What was the reason for the decision to NOT assign Mana to nodes processing transactions? Why should someone be able to assign Mana to another entity?

* Is a node able to determine whether the issuer of a transaction would credit it with Mana before accepting and relaying a transaction (Is the Mana designation part of the transaction?). Is that property signed? If so, how costly is it for the node (wrt DoS) to resolve it synchronously so that it can possibly reject the transaction and the user can find out about it?

* Are node responses (accepted tx, rejected tx, etc) part of the protocol?

* If majority of manaholders does not accept the tx, does it get censored? Similar to pos when majority of stake wants to censor they can. Is Coordicide censorshipresistent at the end?