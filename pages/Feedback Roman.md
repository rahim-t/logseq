---
title: Feedback Roman
---

## (EOS developer in Lviv)

## Let's call the project idea "Mutual Aid Chain". I LOVE the idea. Dan Larimer, the libertarian creator of EOS has talked about Mutual Aid Societies. I thought a lot about it in the early days of EOS, but sort of got lost in the day to day minutia.

## **Initial plan:**

## Let's refine the idea somewhat. I think that'll be a good exercise for all of us, whether we pursue it into the future or now. We can then decide if anyone is serious about execution. If we reach that stage, Rahim, and you are serious about moving forward, we will likely ask for some payment to write a detailed technical specification.

## **Discussing the initial vision:**

## Rahim's initial vision is below wiith my comments marked in blue:

## Oleh, Rahim had discussed one community of several thousand people only. Also, it's significant to keep in mind one of the last bullet points here: "Platform has no name, no marketing, no legal person, no locations, no staff, only shareholders on platform."

## Let me try to give a brief description of the functionality I have in mind:

## Rahim, we will be speaking from the assumption that an EOSIO blockchain will be the best technology for such a multi-faceted project. We can start a separate thread about this assumption.

## Digital mutual aid network for international entrepreneurs to solve the trust problem of distributed cooperation. Market place and information exchange.

## "Information Exchange" - This sounds like some sort of forum that exists on chain. If people can post "pseudonymously", ie. using their main account names it is pretty easy to build. If they want to post completely anonymously, it requires some technical consideration. Allowing users to create disposable accounts for the purpose of posting may be a good compromise.

## "Marketplace" - for real goods? For services? This needs more thought because the delivery of goods/services exists off chain. Is there a reason the forum is insufficient? People will simply find each other and make coordinations off chain.

## Coordination tool for agile projects.

## There are very sophisticated off chain tools like Atlassian Jira, Trello, Slack. Building an on-chain tool has the following risks:
### people are accustomed to existing project management tools. They may not want to switch.

### if we build a tool inferior to the off chain tools, people will not want to use it.

### Blockchains are usually public. It will take extra work if we want to hide project data from public view.Liquidity management inspired by old bills of exchange. Platform is itself first business use case of platform.

## Can we assume that bills of credit need a human manager to decide to grant the bill or not? I think it does.

## Oleh and I built a prototype system called "[Deru](http://deru.io/)":

## Users lock up value under the control of a Judge. Judges have the possibility of offering their service for free or specifying a fee. We were looking for about $40k to build the final version.BTW, Bills of Credit are transferable. This was not part of the plan for Deru, but it could be.

## Reputation management with different balances: "Wisdom" (useful/helpful information and advice),

## I assume wisdom ratings will come exclusively from the forum. For all of these values we have the problem of people faking data by creating multiple accounts and rating themselves.

## "Honour" (track record of honoured liquidity offers), “Skill” (proven product development value to agile teams).

## What if project management happens off chain? I think it's a risky assumption to think people will want us to use a brand new PM tool that we build ourselves.

## “Verified anonymity” to protect entrepreneurs in risky/shut off jurisdictions and whistle blowers on real circumstances on the ground (corruption, risks, ...) and to encourage cooperation between entrepreneurs in mutually hostile jurisdictions. Decentralized platform to eliminate third-party trust. No single back-end, all data should be either in blockchains or sharded distributed hosting. Front-end as desktop app to be downloaded via torrent (for example). • Function priorities 1. Anonymous accounts with key to reputation wallets and referrals

## Can people create multiple accounts?

## Psuedonymous? Or fully Anonymous? Pseudonymous means an account name that is hard to trace to real identity. Fully anonymous is technically difficult, though not impossible.

## Trading (Honour) with liquidity advances ([[Trust]]). Typical trades: Cryptocurrencies, cash, shared private accomodation around the world, bank transfers against invoices, jobs (to be done by currently idle employees or freelancers) …

## What valuable, tradable monies exist on our chain?
### maybe we will have our own token which has a market value?

### maybe we can implement some stable coin?

### maybe other cryptocurrencies will be able to be traded on top of EOSIO - especially bitcoin.

### maybe transfers of value will happen on other chains, or off-chain, and the Mutual Aid Society will rely on oracles.

## Company platform (Shares)

## Governance of the whole chain? Or of communities that exist on the chain?

## Forum (Wisdom) with fine-tuned visibility and bounty incentivation 5. Judgement (conflict resolution, reviews, distributed verification…) - separate function or integrated?

## Governance has a justice system.

## Product developer matching (Skill)

## There's project called HireVibes which is building a decentralized hiring platform on Crypto. There are also other crypto currencies trying to be bounty programs - Bounty0x, built on Ethereum.

## • Balances 1. [[Trust]] = Currency/Payment/Settlement token 2. Credit (Created on platform) = Advance [[Trust]] to be repaid 3. Shares (in companies/projects governed on platform) 4. Honour (Reputation for honoured promises in trade) 5. Wisdom (Reputation for information value and judgment) 6. Skill (Reputation for product development skill and job completion) • Risk to users limited by 1. Cryptography (all ledger entries encrypted), zero-knowledge proofs 2. Decentralization of data 3. Deletion of data after verified settlements, only tokens remain

## Unless we implement heavy anonymizing technology (ring signatures), then information about all historic transactions remain on the blockchain. It may be cheaper to rely on throw-away accounts than to implement the anonymizing technology which is still being developed on many fronts.

## Legitimate use cases dominant 5. Personal referrals limit user base to like-minded entrepreneurs (no criminals) 6. Visibility of offers and information can be fine-tuned to own preferences 7. No p2p interaction outside of trades (to prevent unnecessary identity reveal and targeted scams or spamming) 8. Distributed verification through “oracles” (to verify real-word data)

## Are oracles automated or do we use trusted humans?

## Distributed [[conflict resolution]]Deru ? 10. Only win/win interactions (double coincidence of voluntary agreements) 11. No user names/avatars, users only linked to reputation tokens

## No account names at all? Not even pseudonymous ones? This is a big, and technologically heavy requirement.

## How do users identify each other? Or do they NOT identify each other - they only know each other as "anon with reputation X wisdom, Y honor, etc..."

## Platform has no name, no marketing, no legal person, no locations, no staff, only shareholders on platform.
