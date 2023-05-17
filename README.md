# Common fork bugs

## Compound

- CREAM: flashloan attack & reentrancy with ERC777-like token (no checks-effects-interaction protection) [Postmortem](https://medium.com/cream-finance/c-r-e-a-m-finance-post-mortem-amp-exploit-6ceb20a630c5) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20210830-cream-finance---flashloan-attack--reentrancy)
- CREAM: Price manipulation [Postmortem](https://medium.com/immunefi/hack-analysis-cream-finance-oct-2021-fc222d913fc5) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20211027-creamfinance---price-manipulation)
- Lendf.me: Flashloan and reentrancy (no checks-effects-interaction protection) [Postmortem](https://medium.com/dforcenet/a-summary-of-the-attack-on-lendf-me-on-april-19-2020-e2f1c5d96640)
- Compound: Double-entry point token issue [Retrospective](https://blog.openzeppelin.com/compound-tusd-integration-issue-retrospective/) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20220322-compoundtusdsweeptokenbypass)
- Lodestar Finance: Exchange rate manipulation [Thread](https://twitter.com/BowTiedPickle/status/1601650177369993216) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20221211---lodestar---flashloan-price-manipulation)
- Agave Finance: Flashloan and reentrancy on gnosis, where native token has callback hook (no checks-effects-interaction protection) [Postmortem](https://medium.com/immunefi/a-poc-of-the-hundred-finance-heist-4121f23a098)
- Hundred Finance: Flashloan and reentrancy on gnosis, where native token has callback hook (no checks-effects-interaction protection) [Postmortem](https://medium.com/immunefi/a-poc-of-the-hundred-finance-heist-4121f23a098)
- Ola Finance: Flashloan and reentrancy (no checks-effects-interaction protection) [Postmortem](https://medium.com/coinmonks/ola-finance-hack-a-post-mortem-analysis-7bf498f73a54)
- Rari Capital: Flashloan and reentrancy (no checks-effects-interaction protection) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20220430-rari-capitalfei-protocol---flashloan-attack--reentrancy)
- Venus: Chainlink LUNA oracle became inaccurate during the Terra collapse, which cause a similar result as oracle manipulation and led to draining of protocols [writeup](https://rekt.news/venus-blizz-rekt/)
- Hundred Finance: Exploit of empty markets [Postmortem](https://blog.hundred.finance/15-04-23-hundred-finance-hack-post-mortem-d895b618cf33) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20230415-hundredfinance---flashloan-exchangerate-manipulation--erc4626-inflation-attack)
- 0VIX: price oracle vulnerability allowed donation-based price maniulation [Thread](https://twitter.com/peckshield/status/1651923235603361793) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20230428-0vix---flashloan-price-manipulation)

## Uniswap v2

- Uranium Finance: bad k-value [Postmortem](https://medium.com/immunefi/building-a-poc-for-the-uranium-heist-ec83fbd83e9f) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20210428-uranium---miscalculation)
- DDC: bad k-value [Thread](https://twitter.com/BeosinAlert/status/1564240190851383302)
- Swapos: bad k-value [Thread](https://twitter.com/DeDotFiSecurity/status/1647536474349338624) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20230416-swapos-v2----error-k-value-attack)

## Balancer

- Balancer: deflationary token can drain pools [Postmortem](https://medium.com/balancer-protocol/incident-with-non-standard-erc20-deflationary-tokens-95a0f6d46dea)
- Sentiment: read-only reentrancy [Postmortem](https://hackmd.io/@sentimentxyz/SJCySo1z2) [forum](https://forum.balancer.fi/t/reentrancy-vulnerability-scope-expanded/4345) [POC](https://github.com/SunWeb3Sec/DeFiHackLabs#20230405-sentiment---read-only-reentrancy)
- Balancer: Double entrypoint token DoS risk [Forum](https://forum.balancer.fi/t/medium-severity-bug-found/3161)

## Curve

- Curve: read-only reentrancy [Postmortem](https://chainsecurity.com/curve-lp-oracle-manipulation-post-mortem/)

## Aave

- Aave V2: risk of price manipulation can lead to accumulating bad debt [Governance proposed mitigation](https://governance.aave.com/t/arc-risk-parameter-recommendations-for-aave-v2-eth-2022-11-22/10757/27) [writeup](https://medium.com/@eigenphi/an-in-depth-analysis-of-how-aaves-1-6-million-bad-debt-was-created-ab74027ea108)
- Blizz Finance: Chainlink LUNA oracle became inaccurate during the Terra collapse, which cause a similar result as oracle manipulation and led to draining of protocols [writeup](https://rekt.news/venus-blizz-rekt/)
