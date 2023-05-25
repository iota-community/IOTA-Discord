# Tips to understand the status of your wallet:

This is a collection of information to help our users understand the status of their IOTA 1.0 wallet

- [IMPORTANT INFORMATION - READ BEFORE PROCEEDING](#important-information-read-before-proceeding)
- [How do I migrate from the IOTA Light Wallet to Trinity or Firefly](#how-do-i-migrate-from-the-iota-light-wallet-to-trinity-or-firefly)
- [Differences between a wallet account with a correct seed and a new seed](#differences-between-a-wallet-account-with-a-correct-seed-and-a-new-seed)
  * [Address list of a correct seed](#address-list-of-a-correct-seed)
  * [Address list of a new seed](#address-list-of-a-new-seed)
- [Correct but unused account a.k.a. Snapshot Transition](#correct-but-unused-account-aka-snapshot-transition)
- [Reclaim](#reclaim)
- [iotaseed.io or online seed generator scam](#iotaseedio-or-online-seed-generator-scam)
- [Trinity Incident](#trinity-incident)
- [Wallet migration following the Moonpay incident](#wallet-migration-following-the-moonpay-incident)
- [Wallet NOT migrated following the Moonpay incident](#wallet-not-migrated-following-the-moonpay-incident)
- [Ledger Nano S or X issues](#ledger-nano-s-or-x-issues)
  * [I have lost the index](#i-have-lost-the-index)
  * [Trinity gives an error](#trinity-gives-an-error)
- [Zero funds - LAST RESORT](#zero-funds-last-resort)
- [Exchange Issues](#exchange-issues)
- [YDX](#ydx)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## IMPORTANT INFORMATION READ BEFORE PROCEEDING

IOTA is a decentralized, permissionless, free, and open cryptocurrency. In other words, "you are your own bank". As a consequence the IOTA Foundation and it's members cannot provide user-level support. While we'd love to help every single early adopter, it would simply exceed the available resources. 

## How do I migrate from the IOTA Light Wallet to Trinity or Firefly

The IOTA Tokens are not directly in your wallet but reside on the IOTA Tangle. With your Seed (private key) you gain access to them, to move them around between addresses in the network. Hence you can access your tokens from the Trinity wallet with the same seed you used for the previous IOTA Light wallet.  
Please note that the development of the light wallet is deprecated and it should **NOT** be used.  
Download the latest Trinity Wallet Version from here: https://trinity.iota.org  
In case your previous light wallet seed is shorter than 81 characters please fill up the remaining characters with **9** until you have 81 characters.

## Differences between a wallet account with a correct seed and a new seed

### Address list of a correct seed
- If the **Address List** in Trinity looks like this, it is a seed with incoming and outgoing transaction history

  ![image-20210110205421887](/_resources/images/help/image-20210110205421887.png) 

### Address list of a new seed
  If the **Address List** in Trinity looks like this, then it looks more like an empty wallet

  ![image-20210110205633372](/_resources/images/help/image-20210110205633372.png)

- Make sure to double/triple check if the seed is correct. By typing one wrong character an empty wallet will open. It is possible to use the following community tool to look for a typo in the seed.

  :warning: THIS TOOL IS A COMMUNITY TOOL AND IS NOT ENDORSED BY THE IOTA Foundation.  
  This tool also requires an Address where your tokens are, please make sure to have an address at hand where the tokens reside. It is possible to look at the exchange withdrawal history where the tokens have been retrieved:
  https://github.com/FVANtom/find-typo-in-iota-seed
### How to find an IOTA address on Bitfinex

Exchanges are required for AML reasons (Anti Money Laundering) to keep financial  records for five years. Therefore it should be possible to find an address in your withdrawals list.  
Follow the official guide from Bitfinex to get a report:
https://support.bitfinex.com/hc/en-us/articles/115003361173-Trade-Order-Reports
and make sure that the dates are selected (by clicking on them) like in this picture here:
![bitfinex-history](/_resources/images/help/bitfinex_history.png)

  
### Correct but unused account a.k.a. Snapshot Transition

- If the seed has less than 81 characters, one can pad the number `9` at the end of the input until the seed is 81 characters 
- If the seed is 100% correct and the tokens were not moved for a long time (1-2 years) then:

  **A)** Set Trinity to the following node settings, follow the settings top to bottom, so, disable **Automatic node management** first and go from there and in the end click on the **Save** button on the bottom of the screen 

  ![image-20210110184645086](/_resources/images/help/image-20210110184645086.png)

  
  Then click on the **Snapshot Transition** under the Account **Tools** until the tokens are available in your account:

  ![image-20210110174331122](/_resources/images/help/image-20210110174331122.png)

## Reclaim

  **B)** Please verify an address (from an exchange or similar) on https://explorer.iota.org  to see if the tokens are still there. 
  -  If the explorer shows 0 balance and there are also **outgoing** transactions then it is necessary to follow the outgoing transactions
  -  If the explorer shows 0 balance, AND there are **no outgoing** transactions, then it might be a reclaim case. It is possible to search your address and compare it with the list on the following page for a first assessment.  
  :warning: THE LIST CONTAINS ONLY ADDRESSES WITHOUT CHECKSUM. Should the address have 90 characters, make sure to remove the last 9 characters from the address that is being compared  
  https://gist.githubusercontent.com/cyclux/2bb05d873c4ec6115cad1d100263d489/raw/612a49e46091586957448f6606ea981ab18022e7/snapshot_validation_20171023.txt
  
  - If the text near the address says **AVAILABLE** then it is possible to access the tokens by inserting the correct seed into Trinity
    ![image-20210111085102865](/_resources/images/help/image-20210111085102865.png)  
  
  - If the text near the address says **KEY_REUSE** or **CURL_NOT_TRANSITIONED**
  
    ![image-20210111085016773](/_resources/images/help/image-20210111085016773.png)  
    Please send the **address** (WARNING: NEVER SHARE THE SEED) to the IOTA Foundation for further verification and confirmation.

  Example of an **address** that needs to be reclaimed. The Balance shown in 0. There is **only an incoming transaction** AND **no outgoing transactions** with ##.## MIOTA.
  ![image-20210110180647260](/_resources/images/help/image-20210110180647260.png)

## iotaseed.io or online seed generator scam
- Did the tokens move away between **January 2018** and **January 2019** and the seed was generated using iotaseed.io, then it is a theft case from the iotaseed.io scam.

### UPDATE 25th May 2023
  Dear all,
  I totally understand the frustration that many of you will be feeling around returning the stolen funds to you.  
  This is proving far more complex and complicated than anyone envisaged.
  The issue is MONERO.
  
  When SEROCU seized cryptocurrency from Bitfinex the vast amount of the funds were in MONERO. 
  
  In the UK the Financial Conduct Authority (FCA) has declared that MONERO seized by Police should be destroyed.  They will not allow any cryptocurrency exchange to trade, convert or realise MONERO. 

  To be explicit:
  - We cannot return funds to you in MONERO  
  - We cannot at this time covert the MONERO into another cryptocurrency to then return to you
  - We cannot at this time realise the MONERO into sterling to then return to you
  
  Doing any of the above I will be committing money laundering offences.
  As the senior investigating officer for Op Hyphen this blanket decision by the FCA in my opinion is incorrect.  The FCA have not considered the situation where the Police have seized stolen MONERO belonging to victims of the crime. 
  
  My team are working on reimbursing your all.  They are working extremely hard to come up with a solution.  This involves lengthy and complicated discussions with the FCA, National Police Chiefs Council, the NCA and cryptocurrency exchanges that are or might be willing to assist. 
  I have said on many occasions that we are nearing a solution only for another issue to crop-up.
  Please understand that my primary objective and that of my team is to return these stolen funds back to you. 
  I am not able to provide timescales of when we will resolve this issue. 
  Please can I continue to ask for your patience.
  
  Kind Regards
  Rob


### UPDATE 28th January 2023
  [Man jailed for £2m cryptocurrency theft](https://serocu.police.uk/man-jailed-for-2m-cryptocurrency-theft/)

### UPDATE 8th April 2022
  Message by Demolux_D1#1694
  Hi there! Just a quick update to the iotaseed.io scam (aka online seed generator scam): The trial has been postponed until 25th January 2023. If someone of the according github-page sees that please update this info there.
![image](https://user-images.githubusercontent.com/7383572/162420116-0a1334a7-f7de-46f3-a8e8-20fc30d8d816.png)
  
### UPDATE 26th November 2021
  Message by Koen on Discord  
  ![image](https://user-images.githubusercontent.com/7383572/143553341-e4e2389b-7608-4f2a-8ae2-38eda6e2e89e.png)

### UPDATE 28th July 2021
  Community member message on Discord  
  ![image](https://user-images.githubusercontent.com/7383572/127305878-bda589e1-9a30-473c-9ed3-586222f31717.png)
  
### UPDATE 20th July 2021
  YouTube: LIVE AMA - Seeds, Security and Cybercrime - with Dominik Schiener, Koen Maris & Robert Bryant
  https://www.youtube.com/watch?v=lpPqvcsuwGM

### UPDATE 8th April 2021
  Tweet: https://twitter.com/iota/status/1380166277747126275  
  
  Victims need to report to their local Police station. The local Police will then know the process of going via their Legal Prosecutor to make contact with the UK or they will go via Europol or Interpol.  
  
  The information that you will need to provide is:  
  •Full name  
  •Date of birth and place of birth  
  •Full address  
  •Contact telephone number  
  •Email address  
  •ID Document  
  
  **Details required from officer/staff**  
  The contact details of the representative taking the statement, to include name, email address, telephone number, and address of their police station
  
  **Suggested questions for victims (not exhaustive)**
  1. Detail previous knowledge / experience of cryptocurrency
  2. How did they become aware of IOTA and the seed generator?
  3. Which seed generator was used?
  4. Did they get any encouragement from another user to use www.iotaseed.io ? If so, who? When, and how, was this communicated?
  5. Proof of purchase of IOTA, to include all addresses affected, dates/times, screenshots, photographs, edited statements and if possible also in electronic form
  6. How, when and what quantity was moved? How much does this equate to in losses(specify fiat currency)?
  7. Theft. When did they notice IOTA had been moved? How did they become aware? If they became aware during the unauthorised movement, did they attempt to prevent it?
  8. Seed Security. In regards to security of the seeds, were they: printed out and left in public view; stored in plain text on devices, or shared with anyone else?  If so,  who?
  9. In regards to device security, do they have the latest software installed, latest anti-virus checkers?
  10. Confirmation as to whether they gave anyone authority to move their IOTA on their behalf?  If yes, to whom did they give authority?
  11. What impact has the loss had on them?
  12. Any other questions the statement taker considers relevant to the investigation.
  
## Trinity Incident

- Did the tokens move away between the **12th December 2019 and the 12th February 2020**, the user might be a victim of the Trinity Incident, that involved the theft of the seed during the time Trinity integrated the Moonpay services. In that case send the address to the IOTA Foundation for further verification. (More information here: https://blog.iota.org/trinity-attack-incident-part-1-summary-and-next-steps-8c7ccc4d81e8)

## Wallet migration following the Moonpay incident
- Did the tokens move away between the **29th February 2020 and the 10th March 2020**, then it looks like the user was aware of the theft and did the migration using the migration tool (https://blog.iota.org/seed-migration-tool-now-available-c253ccd9d23c/). In this case there should be a SeedVault.kdbx and a journal.log file on their system. Make sure now to add the password protected SeedVault to Trinity. Be aware that the SeedVault file is password protected that has been chosen by the user during migration. Without the password it will not be possible to recover the tokens. This video shows the whole migration and how to add the SeedVault to Trinity (https://www.youtube.com/watch?v=mjex3IU44VY)

## Wallet NOT migrated following the Moonpay incident
- Did the tokens move away **on or after the 11th March 2020**, then the user did not follow the migration, the seed might have been part of the aforementioned incident and the tokens have been stolen. In this case we encourage users who have had tokens stolen to file a report with their local police and to cite the following case number when doing so: LKA Berlin, Center for Cybercrime, case number: 200213-1717-i00290.

## Ledger Nano S or X issues
- Make sure the same account is in use (24 words, mnemonic recovery words) as when it was set up the first time
- The **INDEX** is fundamental to load the correct IOTA Seed.  
Your Ledger * index = unique seed.  
Ledger * index 0 will generate seed ABC *while*  
Ledger * index 10 will generate seed XYZ
- Make sure you use the original USB Cable if possible. Don't use a USB HUB or USB ports on the display/monitor/keyboard but **connect it directly to your system**
- Close all applications that can access the Ledger device e.g. Ledger Live, Browsers with metamask or the Brave browser
- Remove the Ledger device from the Windows Device Manager (right-click > uninstall device), unplug it, reconnect it and let Windows install the drivers again

If you still experiencing issues with the Ledger, please follow the following procedure:
Close everything on your computer. This includes Ledger Live which should not be running at the same time as Trinity.
Plugin your Ledger. Unlock it with your passcode. Browse to the IOTA App on your Ledger and enter the app.
Now start Trinity and try setting up your account again.

### I have lost the index
:warning: THIS TOOL IS A COMMUNITY TOOL AND IS NOT ENDORSED BY THE IOTA Foundation and will **break the security** of using a hardware wallet.  
This tool is made to find the correct Ledger account index in case you forgot to write it down.  
https://github.com/HBMY289/iotaLedgerIndexFinder

### Trinity gives an error

If Trinity shows the following error or *Invalid bundle* in the Error Log, please read the following guide:  
![](https://miro.medium.com/max/2618/1*GpJag1JbcVDoK4DGRZlBUg.png)  
Have a look at this guide by HBMY:
https://medium.com/@hbmy289/how-to-access-iota-funds-spread-over-too-many-inputs-on-ledger-nano-s-74708548fa6e

## Zero funds LAST RESORT
This step is to be seen as **LAST RESORT** if after tryng all of the above the funds are not available.  
:warning: THESE TOOLS ARE COMMUNITY TOOL AND ARE NOT ENDORSED BY THE IOTA Foundation.  

### OPTION A) HBMY's iotaZeroBalanceHelper
:warning: THIS TOOL IS A COMMUNITY TOOL AND IS NOT ENDORSED BY THE IOTA Foundation.  

_The following information has been taken from the original repository_
This program was written to help Iota users who unexpectedly see a zero balance in their Trinity wallet. There are multiple reasons why this could be happening and often it is not easy for non-experts to find out what is going on.

#### Disclaimer
NEVER share your seed with anyone. No community member or member of the Iota Foundation will ever ask for your seed. If someone does it is 100% a scam to steal your money. That said, even entering your seed into a software other than the official Iota wallet should not be handled lightly and can only be recommended as a last resort. For your own safety you should run this software only an an air-gapped computer. 

#### What does it do?
The goal is that the program lets unexperienced users test what could possibly cause Trinity to not show the expected balance. I plan to add more tests over time.
The program allows to 
1. check if funds on addresses of a seed were taken into custody by the Iota Foundation in late 2017. If this is the case the affected funds are reclaimable.
2. check if there is any balance that Trinity might not show. The program will list all addresses with balance while Trinity will often only show a single address if no funds are found. 
3. export a list of generated addresses to be tested with the online tool [iotaAddressHistoryChecker](https://github.com/HBMY289/iotaAddressHistoryChecker)
4. check for typos in the seed (not implemented yet)

Seeds that are too short or too long will be adadpted in the same way the Iota Light Wallet did.

##### Reclaim
With the given seed the programm calculates a large number of addresses both using the current address generation algorith and the one that was used in 2017 and earlier. These addresses are then matched against a list of reclaimable addresses. Possible matches and reclaimable balance will be shown. If no match is found using the Iota reclaim process will NOT bring back your balance.

##### Balance
If a reclaim case could be ruled out, the balance option will generate addresses using the current algorithm and compare them to an internally stored snapshot of the tangle. This snapshot holds all addresses with balances and by matching against this list the program does not need any connection to the internet or the current tangle to check balances. Currently a snapshot file from Feb 12th, 2021 is included. If you are missing a funds that have been moved after this date you can supply a more recent snapshot file. Ask someone who has access to a Iota node to run the following command and supply you with the resulting file.
```
curl -H 'X-IOTA-API-VERSION: 1' -d '{"command":"getLedgerState"}' localhost:14265 >  snapshot.txt
```
Place the file `snapshot.txt` next to this tool's executable. It will be automatically be used when checking the balances.

##### Export Addresses to check online
This program requires to enter your seed and is designed to run without any internet connection. If all your addresses still do not show any balance you can check the addresses on the Iota tangle explorer [https://explorer.iota.org/legacy-mainnet](https://explorer.iota.org/legacy-mainnet) for any transactions that show where your funds went. To avoid having to enter all addresses manually I wrote another tool that automates this process ([iotaAddressHistoryChecker](https://github.com/HBMY289/iotaAddressHistoryChecker)). It will require a list of addresses exported by the iotaZeroBalanceHelper and then request all available tranascations from the explorer. It will report any token movements in a short and human readable report.

**Finally HBMY's iotaZeroBalanceHelper is available here**: https://github.com/iota-community/iotaZeroBalanceHelper/releases

### OPTION B) FVANtom's IOTA seed typo finder
:warning: THIS TOOL IS A COMMUNITY TOOL AND IS NOT ENDORSED BY THE IOTA Foundation.  

_The following information has been taken from the original repository_
##### WARNING

NEVER give your seed to anyone, not even to someone you think you can trust. Not even the devs. There's scammers out there. NEVER enter your seed into or download any software that is closed source and/or that hasn't been reviewed and approved by either the IOTA foundation or at least the IOTA community.


#### What does this tool do

I have written this tool to help a user on Reddit who accidentally made a typo in his seed while logging in into the wallet.

He then transfered iota to the address he generated and logged out of his wallet.

Because he accidentally made a typo when logging in, he lost access to his funds.

This program checks the most common typing mistakes and tries to find the real seed (typo-seed) of the address the funds were transferred to.

* Generating seeds with one missing character readded
* Generating seeds with one character missing
* Generating seeds with character typed double
* Generating seeds with letters that look like each other replaced
* Generating seeds with block of 2 character retyped
* Generating seeds with 2 neighbouring characters switched
* Generating seeds with 1 character mistyped

#### Who is this program useful for

Anyone who transferred funds to an IOTA address of a seed similar to his own but with a typo and doesn't know the 'typo-seed'.

#### To use this program you will need:

* Your original seed
* The address your funds were transfered (belonging to the 'typo-seed')

**Finally FVANtom's IOTA seed typo finder is available here**: https://github.com/FVANtom/find-typo-in-iota-seed/releases

## Exchange Issues
- Something with my IOTA transfer went wrong, my Tokens did not arrive from an Exchange
- My exchange does not credit my IOTA tokens
- Were the funds sent to an exchange twice to the same address?
- Were funds withdrawn from an exchange and are still not in your wallet?  

IOTA is a permissionless protocol. As such, we are unable to interact with the transfer between you and your exchange. Please contact the support of your corresponding exchange.

- How do I withdraw from my exchange?  

Your exchange should provide this information as part of an FAQ or similar. Please not that we are not able to provide specific withdrawal instructions for IOTA tokens for every IOTA trading exchange.

## YDX
This is the message by YDX posted to the IOTA Discord.  
Direct link to the message: https://discord.com/channels/397872799483428865/398499876935303186/818548205372964884  

_"Hi, so a quick message here because I see some people complaining and maybe mods can send them to this post in the future. Ydx closed a year ago after a 2 years shutdown notice with monthly, then bi-monthly channel notifications. It was initially a 1 year notice but considering the balances left, we gave another 1 year for users to withdraw before it shuts down. I logged back into Discord a couple weeks ago because, with the price development, some people might have shown up eventually. I had 3 dm's and 2 of them are sorted. They might feel free to confirm that here, it's not from me to say what has been sent to who. Why did it close? There was 0 activity and if minus was available, we would have been there. People think it costs nothing to store large amounts, they couldn't be more wrong. If we've been successful at escrowing large amounts, this is mainly due to our process and the platform never got hacked or scammed. So at some point, after 2 years tagging people constantly, you shut everything down... especially considering the small amounts left overall. Or you just wait for 1 message per year while maintaining at an important cost. Obviously not counting the money we also invested for the discord bot also and that barely no one has ever used and Slack free plan as well which keeps no history and makes it extremely difficult to keep track of messages and activity. I don't like being called names when we gave such a long notice, especially when such cases happen in the industry and a provider shuts down, they will give you a 2 weeks notice. But it's fine, I guess it's part of the process where people will judge us responsible for their inaction. Feel free to dm me but don't even try to impersonate other users, we know exactly how to identify the legit users. Be aware I barely never log into discord so if I don't reply right away, no I'm not gone, I'm just not here._

Message screenshot:
![](https://i.imgur.com/ohDEzVM.png)
