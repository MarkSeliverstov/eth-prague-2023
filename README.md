# eth-prague-2023

## Project Description

The application is using ENS names with account abstraction to simplify UX and allow for a more secure experience and accessibility. When combined with account abstraction, users can seamlessly utilize ENS names in their interactions, abstracting away the complexities of handling Ethereum addresses directly.

## Problem

Wallet social recovery is a mechanism that allows users to regain access to their wallets by leveraging a network of trusted contacts. In this approach, users designate a group of trusted individuals who can collectively assist in recovering the wallet in case of loss or forgotten credentials. When the user initiates a recovery process, the wallet sends notifications to the trusted contacts, who then provide their approval or assistance. Once a sufficient number of trusted contacts validate the recovery request, the wallet grants the user access to their funds and account, effectively restoring control over their assets. This method enhances security and provides users with an additional layer of protection against the risk of losing access to their wallets.

Currently users have to add a fixed wallet address (like 0xycc...) of their guardians. Later during the recovery phase the Guardians (owner of the guardian addresses) have to approve the recovery by sigging the recovery request via the originally specified addressed.

The problem is that for different reasons guardians may loose access to the originally specified ethereum address. For example, they decide to migrate all their assets form one wallet to other wallet and forget to track all references to the old ethereum address. 
