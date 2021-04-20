# Hello IOTA Community!
# Have a look at this draft and contribute to the FAQ by adding your questions here: https://forms.gle/5amEK4BqJ1b5FaQr8
  
  
  
  
  
## I have migrated the tokens, now what?
The migrated tokens will be available in Firefly starting 28 April 2021. Before that date, the tokens are locked and further transfers are not possible.


## What if something goes wrong while I migrate? Who do I contact?
If any part of the process is aborted or fails, it can be redone! If something still goes wrong, reach out to the #help channel on [discord](https://discord.iota.org) for community support.  
**IMPORTANT**: Never share personal information regarding the amount of tokens you own, their type, or where and how you keep them, how you secure them including passwords, recovery passphrases, and user names of wallet accounts or exchanges. Do NOT share that information with anyone - including members of the IOTA Foundation.
[Read more about Chrysalis “Security During Token Migration”, here](https://blog.iota.org/security-during-token-migration/). 


## If I have multiple addresses associated with one seed, will the Chrysalis migration amalgamate all of my tokens to one address?
Firefly will attempt to consolidate all of your funds but there is a chance some dust (<1 Mi) is lost.


## As I understand dust protection, in Chrysalis, it will no longer be possible to have seeds that contain <1 Mi? So what will happen if I try to migrate those (I have a few of them)? Will I have to make sure all these seeds get consolidated before Chrysalis launches? Or will Firefly support migrating x old seeds into a single new one?
Seeds and also single addresses that are a part of Seeds with <1 Mi balance are considered dust and will not be able to migrate. We recommend sending all of those small balances to 1 new address on a new seed to consolidate them and reach a balance of >=1 Mi on this new address. This address can be migrated without issues.


## Will the Firefly mobile app be available upon Chrysalis release or do I have to migrate on PC?
For now, the migration will be done via PC. [Once the migration is complete, we will shift our focus to the mobile app!](https://blog.iota.org/chrysalis-network-migration-release-date/)
The following options are available should you be interested in trading the IOTA tokens right after the migration to Chrysalis:
- Migrate your seed using a Desktop PC/Notebook using Firefly between 21 April 2021 and 28 April 2021
- Send the tokens to an exchange that supports Chrysalis prior to 28 April 2021 and let them migrate the tokens for you, then wait for the Firefly mobile version


## I use a Ledger Nano S / X, are there any special things to take into account using a Ledger at the transition?
We have made the decision not to include Ledger Nano migration in the first Firefly version. Ledger Nano migration will be available in Firefly v1.1 soon after the Chrysalis upgrade. While the Ledger implementation is more or less ready, we do not want to rush its testing and deployment. 
If any Ledger Nano users do not want to wait a couple of weeks and need to access their funds sooner than it is recommended, then they transfer them to a regular seed before 28 April 2021.
The following options are available should you be interested in trading the IOTA tokens right after the migration to Chrysalis:
- Send the tokens to an exchange that supports Chrysalis prior to 28 April 2021 and let them migrate the tokens for you
- Send the tokens to a Trinity account without Ledger, by setting up an IOTA seed based account and migrate the seed using Firefly between 21 April 2021 and 28 April 2021


## I have 20 addresses on my Ledger Nano S. Is that a problem? I heard about this memory problem where only 2 addresses can be emptied at once.
The migration will bundle addresses together to avoid issues. We encourage you to consolidate the tokens in one address. Have a look at this [article by the IOTA community](https://medium.com/@hbmy289/how-to-access-iota-funds-spread-over-too-many-inputs-on-ledger-nano-s-74708548fa6e) for further information about how to consolidate your tokens.


## What are the tax implications of the migration?
Tax regulations are different from country to country. Contact your local tax office or a tax consultant for the exact handling in your country.

## From what I understand, you need the 24-word recovery phrase to migrate to the new network. But why would you need that recovery phrase, which malware could possibly exploit, if you already bought a Ledger for safety? Do I even need to type in my recovery phrase even if I have a Ledger? Or is there a migration for Ledger users without using the 24-word recovery phrase?
While the 24-word recovery phrase for Firefly uses the same 24-word format as the Ledger, they are actually two different things! Also, *you should never type your ledger recovery phrase anywhere!*  
The 24 words some users currently have for the hardware Ledger *is the recovery phrase to recover their funds for any cryptocurrency (including IOTA) that they use their Ledger for*, should they lose or somehow destroy their ledger.  
The 24 words that users can currently use for Firefly Beta *is the recovery phrase for the software wallet stored in Stronghold*, should they lose their Stronghold backup file or it becomes corrupted somehow.  
[The first Firefly v1.0.0 wallet that is going to be released will not support hardware ledger](https://blog.iota.org/firefly-token-migration/), so if you'd like to trade your tokens before 28 April 2021, you have to send your tokens to a normal seed in Trinity from the hardware ledger before 28 April 2021.  
Additionally, the next Firefly update that comes in a couple of weeks will support hardware Ledgers. You will be able to migrate your funds to the hardware Ledger then.
