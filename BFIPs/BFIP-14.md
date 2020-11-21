## Preamble
    BFIP: 14
    Title: Funding for Development 
    Author: Boosted Finance Core Contributors
    Created: 2020-11-21 (21st NOV)

## Simple Summary

The Boosted Finance team is requesting funding of 90,000 yCRV to fund ongoing development efforts for bVaults, new developers and designers, implementation of strategies, bug fixing, content creators, growth, and partnership developments..

## Abstract

The Boosted Finance team proposes the following measures to be implemented using the funding requested from the treasury:

* 65,000 yCRV to compensate existing and recruiting new developers, UI/UX designers for their time and work in the fairest way possible, development efforts for bVaults, implementation of strategies, bug fixing, enhancing front-end interface among others.
* 15,000 yCRV to compensate for growth and partnership efforts with other DeFi and blockchain projects, exchanges.   
* 5,000 yCRV to be used for server and other development costs, e.g. hosting, domains etc.
* 5,000 yCRV for miscellaneous and unexpected expenses should the need arise (e.g. human resources, recruitment, oracle costs, liquidity pool set up, gas fees, smart contract deployment)

We believe it’s best to allocate adequate funds for the contributing team to align incentive and motivation to support the project at a key stage where DeFi is reaching new all-time highs of $13.62B TVL. This will also ensure resources to support ongoing strategists who participate in the upcoming strategist competition and others who continue to submit proposals for new vaults. 
In addition, this will fund efforts to collaborate with other decentralized finance and blockchain companies to create synergistic value for Boosted Finance. 

For context, governance in v1 batched together logic that handled governance proposals as well as the holding of treasury funds in yCRV. The new release of [BoostGovV2.sol](https://etherscan.io/address/0xd7E6cf7a09DFC8c820f606119e9E5e58e2E34C66#code) and [Treasury.sol](https://etherscan.io/address/0x71151b7AE78459093f1B29583f2B24aEF603cB70) separates the functionality of both to separate  contracts which would have required a coordination effort to migrate old treasury funds. See more details on the updated governance contracts that are currently under audit [here](https://medium.com/@BoostedFinance/boosted-finance-final-pool-distribution-booster-changes-governance-contracts-58e01395d331).
If the proposal passes, the extraction of funds from the treasury will be done in two steps to eliminate the need to migrate the old governance contracts to v2. 

1) 54,266 yCRV will be withdrawn from old treasury [https://etherscan.io/address/0xc3859cb576f7e8a0a8537a5ce4700c95802daf81]
2) 30,734 yCRV will be withdrawn from new treasury [https://etherscan.io/address/0x71151b7AE78459093f1B29583f2B24aEF603cB70]

Upon deployment of the new treasury and governance contracts, we identified a bug that would have allowed anyone to call those functions with arbitrary amounts, and submit and vote for malicious proposals that drain the treasury. We have fixed this by sending a transaction staking the max amount possible uint(-1) to restrict anyone else from staking in the governance contract temporarily as we wait for our professional audit to complete.

## Motivation

Our motivation for submitting this proposal is to ensure enough resources to improve and iterate upon bVaults in the next 2-3 months. With the fair token distribution and initial deployment of bVaults completed, we are submitting this proposal to onboard new resources in development, designers and growth to assist with the project going forward.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
