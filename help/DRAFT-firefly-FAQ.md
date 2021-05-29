# Hello IOTA Community!
# Have a look at this draft and contribute to the FAQ by adding your questions here: https://forms.gle/L9nxek9KonCFvHqw8
  
  
  
  

# Setup and installation
## I’m worried I might make a mistake when setting up Firefly!
Don’t worry! All you need to do is download Firefly only from the official website for your preferred OS and start the setup. The application has been designed to guide you through setting up your account, securing it, [and migrating your tokens successfully.](https://blog.iota.org/firefly-token-migration/)

## How do I back up my seed? 
The IOTA Seed is now a 24-word mnemonic or a recovery phrase. After 28 April 2021, like with other cryptocurrencies, all you will need are 24 words to recover access to your tokens on the Tangle. You will be able to backup your seed using the recovery kit you established when you set up your wallet. By saving a file and writing it down, you will have captured the 24-word recovery phrase in a safe location. 
A physical backup is recommended, like a piece of paper, as computers can fail, and having only a digital copy might be insecure in the long run.
Hardware wallets such as the Ledger will be supported soon after the initial migration period. 


## What is a “Stronghold”?
Stronghold is a secure software implementation developed by the IOTA Foundation with the sole purpose of isolating digital secrets from exposure to hackers and accidental leaks. It uses versioned, file-based snapshots with double encryption that can be easily backed up and securely shared between devices. You can read more about Stronghold [here](https://blog.iota.org/iota-stronghold-6ce55d311d7c/)!


## I have lost access to my device! How do I recover my wallet?
There are several ways to recover your wallet, and both can be found in the backups you performed in the wallet setup! One way would be using your 24-word recovery phrase, while the other would be using the files you backed up in Stronghold.

# Backups and Recovery

## I have the seed words (recovery phrase) but don't remember the password; what can I do? 
The recovery phrase works without a password or PIN! Just input the words at the wallet set up, using the "I have a text backup" option.
![img](https://lh6.googleusercontent.com/EOa8RcGbIV7ir6RfFzPTFkwWuHAQSZVYPW3h5MZLJVe_efBuN-F7VSS9q01rMl4x2wqRiGn4vu-Uts73IwL98cgu5BlCYeAOLE8AHafn5LVybQ-8aJe8qAAeRoEFgzrkppOofmc8)

## I found an old seed from Trinity, how can I access these funds now that the migration period has already finished?
Seed migrations can be made after the migration period ends, at least until [Coordicide](https://blog.iota.org/coordicide-the-road-ahead-7d89f41b0ba5/).


## Why should I do regular Stronghold backups?
Performing regular Stronghold backups will allow you to keep up to date recoveries should something happen, where you would then have a complete recovery of your funds.


## What is an internal transfer? Is it different from a normal transaction? 
An internal transfer is the same as a normal transaction, it’s just made between your own accounts; it's also handled fully on the Tangle. Here, it's simply easier to perform as the address doesn’t need to be input by you!

# Profiles and Accounts

## What are profiles in Firefly?
Profiles in Firefly are representations of your IOTA seed and contain all of your balances on different accounts. They also include general information such as if you prefer a light or dark theme, your language and currency preferences, and system notifications.


## What are accounts in Firefly?
Accounts in Firefly are like a bank account and a personalized stock portfolio all in one! And in that sense, accounts always belong to a specific profile of your Firefly application. You can view your account balance and transactions, send and receive funds instantly, measure your account and token value over time, and check your account activity by month! 
![img](https://lh4.googleusercontent.com/5d6eIXjTxrubrZHkjmMQNMfkApp7wLohTAGv5JZIJJR7lsB7fOwGCsQt9Do1CkVNmhid7_c7aWyTcwRv8dALkvTLeEfBQf7ABmpc1e48N6G3sHz80ZrErOZZU81nNDOlqeKKeA0V)

## Can I change profile names after I created the profile?
No, you cannot change a profile name after creating a profile. But you can add a profile with your preferred name and populate it near instantly with your preferred account(s), security, and other such information.


## Can I change account names after I created the account?
Yes! You can change your account name by clicking on the ellipses (three dots in a row) next to your account balance which will give you the “Customise account” option. There, you can change the name of the account you are currently in! 
![img](https://lh6.googleusercontent.com/nL4B4Cg1tsRzN3ZPTWi8R5DyCYQIs2nvAh-6f4wmpDzfGlEiLNhNk8q7TCIcGSuJWR9swXm29oWnwB0pYlz4r8l7rzcakGi7454Zjmoo9kJolTb8oy_OihLp03qLA6xbmyBwXaTn)


## What is “resync account”? Why do I need it and what happens when I do it?
Resyncing your account starts a background task that makes sure all of your accounts are up to date; you would need it to ensure your account is correct so you can conduct the everyday functions of Firefly without issues!


## I want to delete a profile, what happens to the funds in that profile?
Profiles can only be deleted after your funds have been moved out of your profile. So, you would need to send your funds from that profile to another address. 
However, an empty 0 balance profile can be deleted.

## Can I use my own node to process my transaction? 
Yes! You can use your own node to process your transaction if it is accessible over https.


## How can I reattach transactions?
There is actually no need to do this anymore!


## I accidentally sent funds to the wrong address, can I get them back? 
There is no way to recover funds accidentally sent to the wrong address.


## Why do I need 1 Mi on an account to receive transactions with a value <1 Mi?
Because there is a *minimum* requirement of 1Mi for a successful migration due to IOTA protocol’s [dust protection](https://github.com/GalRogozinski/protocol-rfcs/blob/dust/text/0032-dust-protection/0032-dust-protection.md). It is not possible to migrate a seed or an address with <1 Mi. 


## How can I send data transactions with Firefly?
You cannot send data transactions with Firefly at this point in time.


## Where can I see the history of all my transactions?
Your transaction history is broken down within your accounts. When you select “Accounts” from your dashboard, you will see a column with all of the transactions you made within the respective account. 
Additionally, there is an extra function, “Account history” found in the ellipses (three dots) next to the “Account balance” of your Account page. 


## How do I find a specific transaction that I did send / receive; I only know the day when it happened, is there a search function?
There is no search function in Firefly.


## What is a deep link, and how do I use it?
Deep links automatically fill transaction data in Firefly when you click on an “iota://” link. You simply select the “Enable deep links” option in your “Advanced Settings” to use this feature.
![img](https://lh6.googleusercontent.com/3whrQsl19SL6KITRG_b0kbh_S94I_qyqBDWP2cOORDKYlVLHBcurys5AJl5ubgQAnRK2NQhbpRdV2NlTVgy8opBESM-1S8dUxsNRs2ZGg-_cZRY4EhnKg8LTHcLcH8OOezCNPA-F)


## Can I have a fixed receive address? 
Yes, you can have a fixed receive address! Additionally we are working on a way to streamline making a fixed address because as of right, now you have to enter it manually. 

# Settings

## Where can I change my PIN and password?
You can change both your PIN and password under “Security” found in the “Settings” of your dashboard.
![img](https://lh4.googleusercontent.com/OMOqS3Wd_qSrSn8H5gxsIksRGFxvucBUPtvtNxGtZEUtsTrPCkk2vqFspHte5sQCO7pyNLvZhY5XJXCzqtMoYUiSZcraQv-CEJ5V6jkF2osZxxeDoVsqJ-fIjpF3qIHiPus9dFWv)


## Can I reuse an address? I know in Trinity this was always a problem.
Yes, you can reuse an address based on the EdDSA reusable address format. 


## Can I create NFT’s or other digital assets in Firefly?
You cannot create NFT’s or other digital assets in Firefly at this time.


# Troubleshooting
## How do I recover a PIN code?
If you have lost your PIN, you need to create the profile again from a backup (recovery phrase or a Stronghold file) to access the profile again. Afterwards, you will create a new profile with a new PIN.


## I have my backup file, but don't remember the password, what can I do to recover my funds?
Without the password, you will not be able to recover your funds using the backup file. It *is* possible to recover the access to your funds using the recovery phrase and setting up a new profile in Firefly. However, your Firefly settings and history are lost by doing so.


## I received an error, what can I do?
For any issues or errors, you can report to this github page: https://github.com/iotaledger/firefly/issues


## I received an error: “client error: {}”, what does it mean and what can I do?
For any issues or errors, you can report to this github page: https://github.com/iotaledger/firefly/issues


## I received an error: “operation timed out”, what is it and what can I do?
For any issues or errors, you can report to this github page: https://github.com/iotaledger/firefly/issues


## For those who have more than one seed, can we replicate this process whenever the amount of seeds we have? Or do we need to put all iotas together in one seed in order to do the steps?
You can import multiple seeds in Firefly! But they must be done one by one.


## Can I buy IOTAs directly in Firefly?
You cannot buy IOTAs directly in Firefly at this time. You can visit the [IOTA website](https://www.iota.org/get-started/buy-iota) for more information about buying IOTA from an Exchange.
