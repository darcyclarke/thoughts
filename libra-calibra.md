# Libra & Calibra

So, I've read a lot about Facebook's new "cryptocurrency" & wanted to consolidate some of my thoughts/thinking here. For reference, I've added some of the articles I found most useful, along with the [marketing][1] & [white paper][2] citations, [below](#references--citations).

### Introduction & Overview
At a high level, I've been extremely skeptical about the practical usage of traditional cryptocurrencies (ie. Bitcoin, Litecoin, Etherium etc.) as the fundamental technical underpinning [does not scale](https://www.youtube.com/watch?v=s2XHyzPA9Zc). That said, Facebook's new "cryptocurrency" operates more like what PayPal should have been/become, in terms of a standard interop for digital transactions.

Some of the core concepts I'll touch on & probe are: cryptography, permission, consensus, wallets, decentralization & centralization; In many cases, these terms have grey areas &/or vary in their usage in all the articles I've read or discussions I've participated in over the last few years.

### What Libra is?
- Fiat 
  - Local, "stable" fiat currencies are allowed to be converted, then held in a reserve; Allowing for, potentially, infinite Libra to be in circulation
  - Interest on fiat currency put into the system is distributed relatively between regulators (ie. consider the exchange of cash for Libra as if you were putting money into a savings account which the bank redistributes or gains interest on)
  - The value of Libra isn't dictated by market demand or expectations; Instead, regulated by the "association"
  - Honestly, it seems like a hedge-fund with some central banking concepts thrown in
- Centralized (ie. the "association" acts like a central bank with governance, authority, ledger validation, interest, reserves etc.)
- [Private / Permissioned](6)
- Fast/scalable
  - Having limited nodes/authorities means you can [shard/fork the blockchain][7]
  - You can hit **1000 transactions per second** because of limited consensus & nodes on the network (see "Permissioned")
- No accountability/regulation at the transaction level
  - Wallet/application developers are not vetted/verified
  - Transactions are all irreversible (although, all blockchain cryptocurrencies are like this, it's just a very dangerous precedent to be setting en-masse)
- Will never be recognized by institutional banks/governments (ie. you can't pay your taxes or mortgage with Libra) (*I'm speculating*)
- Restrictive association requirements (ie. becoming a validator/regulator node on the system):

> *"To join the association, members must have a half rack of server space, a 100Mbps or above dedicated internet connection, a full-time site reliability engineer and enterprise-grade security. Businesses must hit two of three thresholds of a $1 billion USD market value or $500 million in customer balances, reach 20 million people a year and/or be recognized as a top 100 industry leader by a group like Interbrand Global or the S&P."*
>
> *"Crypto-focused investors must have more than $1 billion in assets under management, while Blockchain businesses must have been in business for a year, have enterprise-grade security and privacy and custody or staking greater than $100 million in assets. And only up to one-third of founding members can by crypto-related businesses or individually invited exceptions. Facebook also accepts research organizations like universities, and nonprofits fulfilling three of four qualities, including working on financial inclusion for more than five years, multi-national reach to lots of users, a top 100 designation by Charity Navigator or something like it and/or $50 million in budget."*

### What Libra isn't?
- [Public](6)
- Decentralized (ie. in terms of governance, authority, ledger, reserve etc.)
  - Trust is shifted away from the community at large & back to an oligarchy
  - This is less safe then traditional blockchains as the centralization of authority/validation is prone to exploitation
- New currency or wealth
  - There is no way to "mine" or create Libra unless the "association" distributes more (ie. a fiat currency) 

### What Calibra is?
- A managed wallet (ie. you get some degree of safety/support for backups when there is a hack or loss of currency)
  - Unfortunately, you have to provide a means of authentication/identification (ie. passport, license etc.) which concedes any privacy/anomynity to an already disingenuous brand(s) who can't be trusted to keep your data private
- A pseudo-digital bank (much like PayPal)

### What Calibra isn't?
- Private (ex. sudo-nonymous profiles are associated with wallets & meta data on purchases will be captured)

# Conclusion

Overall, Libra is more similar to PayPal, or some kind of freemium game currency (ie. digital "bits"), then a traditional cryptocurrency. Unfortunately, the marketing of Libra is doubling down on hot crypto buzzwords even though the actual offering misses the mark. The attractive part of cryptocurrencies is their radical, & yet, crucial decentralization of authority through blockchain validation. Decentralized wallets mean nothing without a decentralized, authoritive ledger as well.

The success of Libra & Calibra will be determined by the adoption/support amongst the wider marketplace (ex. similar to Apple/Android pay systems). It will almost assuradly take over some marketshare from existing payment processors but I'd be hesitant to say that transferring our trust & control of any currency to corporatations, not governed by states, will benefit end-users/consumers.

### References & Citations
- [Libra][1]
- [Calibra][2]
- [TechCrunch][3]
- [The Verge][4]
- [Bloomberg][5]
- [Permissioned Blockchains][6]
- [Scaling Blockchains][7]

[1]: https://libra.org/
[2]: https://calibra.com/
[3]: https://techcrunch.com/2019/06/18/facebook-libra/
[4]: https://www.theverge.com/2019/6/26/18716326/facebook-libra-cryptocurrency-blockchain-irs-starbucks
[5]: https://www.bloomberg.com/news/articles/2019-06-18/better-than-bitcoin-facebook-unveils-libra-cryptocurrency
[6]: https://www.investopedia.com/terms/p/permissioned-blockchains.asp
[7]: https://www.youtube.com/watch?v=4CdO0olVfAA
