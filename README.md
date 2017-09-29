# Faction

#  ⏳ Contribute to ICO's as a group, in a trustless manner ⏳

![Solidity Password Protection Smart Contract Function](https://cdn2.macworld.co.uk/cmsdata/features/3505364/Portrait-Lock.jpg)

ICO's provide whitelists for favored investors, or friends/advisors. This guarantees them a certain amount of assets to be purchased.
Typically with these whitelists, the allocation is larger than they're able to personally fill, so they will then provide some of the 
allocation to interested parties they know.

ICO Structures differ
- Organized - Accredited sign up, receive verified and unique smart contract address. (Civic)
- Tsunami - One address, flooding in from everyone, everywhere at one time. (Brave browser)
- Time Sensitive Blocks - Allocated an amount that they can purchase when signing up, amount being received will vary based on the time the deposit is made to the ICO.

## Problem

**Technical** 

Groups that are all contributing to a whitelist need two points of trust.

  a) Whitelist person to deliver the tokens.
  
  b) Group organizer to deliver funds to the whitelist.

**Convenience**

Investing in ICO's forces multiple parties in multiple areas of the globe to be ready to go at a time that may or may not be convenient to them.


## Solution

A smart contract that takes the deposits from people, with a fixed destination (white-list, or ICO) to push those deposits too.

All tokens that were received (or to be received) from the ICO will be allocated back to the contract.

Tokens are distributed pro-rata. E.g. 100 people all deposit 1 ETH into the smart contract, the smart contract manages to deposit 90 ETH to the ICO, then everyone gets 1% of the tokens received, and rebated the additional ETH that was not able to be spent.

- Provide a smart contract for the ICO to whitelist (just as they whitelist particular individuals)
- Contract is then loaded up 
This is a very basic example of a smart contract in Solidity that, just like an hourglass with sand, it'll accumulate Ethereum that is available to withdraw over a set time period since the request. The more time that passes, the more that will be released, up until a pre-defined threshold. 

## 👌 **Good use cases** 👌 
- You and your friends are syndicating funds together to send over to one of the syndicates friends

## ⚠️ 🚨 **Bad use case (Don't ever do)** 🚨⚠️

- Put tokens in this contract. You need to add the code for the tokens first, it's ETH only (on this example!)

### *Example:* 

"I'll send my Civic tokens, 0x tokens, and a few others into this contract, cool!"

### *Why:*

It literally is programmed to send out ETH. **Nothing else at all.** Once deployed, and once received by the contract, there's no code telling it what to do with anything other than the ETH. Just an fyi, trying to make sure nobody loses anything valuable of theirs.


### *Comment*

Platforms could adopt a different architecture to the usual balance of hot wallet/cold storage solutions. Including some sort of opt-in for their customers that want that utilize something like this. Some people might feel like multi-sig is a strong middle ground, however I feel like multi-sig security is great, although it's effectiveness is directly correlated to it's inconvenience (the more signers, the more secure, the more inconvenient).


**Hot Wallet** - Vulnerable to the keys being compromized. All or nothing solution.

**Sand Release** - Limited protection from assets compromized keys, and accessibility. Middle ground 

**Cold Storage** - Impractical for accessibility. All or nothing solution.

This was a fun project to do, and would appreciate any feedback as I'm new to writing Solidity! 

Thanks so much :)

Kind regards,

Michael.

