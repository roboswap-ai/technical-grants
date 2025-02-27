# TECHNICAL GRANTS APPLICATION TEMPLATE

***Instruction***

*This application is comprised of 4 sections:*

1. *Project Description*
2. *Team Background*
3. *Development Roadmap*
4. *Additional Information*

*Please complete each section entirely by replacing the block-quotes with your own plain text answers. Applications must be filled completely in order to be eligible for grant funding.*

## 1. PROJECT DESCRIPTION

>Please provide the following:
>- Title and brief description of the project
>- Motivation behind the project (objective / anticipated impact)
>- Why you chose to build on Kadena

### Kaddex SDK

We, the RoboSwap team, as the first step in our vision of becoming a "usability layer for DeFi" are starting by building out the core elements of the DeFi ecosystem, to ensure we will have a sound and reliable base to grow upon. Part of our strategy is to discover up and coming ecosystems which have a high growth and success potential. We have selected Kadena in particular as having the right idea about several important aspects including security, performance, and a brand which is attractive to certain market segments, among other things. In regard to the burgeoning DeFi ecosystem on Kadena, we do see inter-chain capabilities and inter-operability as a strong point. However, we see that it's very important to showcase a full suite of Kadena-native protocols in order to demonstrate the full power of the unique properties of Pact and ChainWeb. As we see it, the core of any DeFi ecosystem starts with a DEX -- liquidity pools, swaps, and other important basics that are familiar and enticing to the large and balooning retail market, as well as larger, more experienced and established players. Kaddex is well-positioned as the flagship DEX on Kadena. We would like to build out several projects over the coming months to ensure Kaddex achieves great success and attracts the use of a large ecosystem of market participants. Projects we envision include SDKs to encourage partnership with and usage by other protocols, as well as the technical infrastructure to maintain highly effective incentive programs for staking (farming) and liquidity pools. As RoboSwap, we also have a keen interest in the ability to develop various tools and technologies for quantitative analysis of market data and automated trading. Finally, we see that the most successful DeFi protocols must understand and leverage the large, and sometimes mysterious or misunderstood, market of arbitrageurs as a core part of their overall strategy. For all of these reasons, we believe the project with the highest ROI for all parties involved would be for RoboSwap to consult and deliver a high-quality SDK and documentation for Kaddex. Therefore, our first proposal is delivery of a Kaddex SDK (version 1). After the first SDK version is delievered, we would propose building on the momentum and expertise of the same team to develop a technological base for highly effective incentivization of market participants to provide liquidity to Kaddex.

## 2. TEAM BACKGROUND

**Team Members**

>For each team member, please provide the following:
>- Structure: Indicate team member roles including who is the team lead and any advisors
>- Background: A concise bio of relevant experience including any previously completed projects
>- GitHub profile link
>- LinkedIn profile link

Jeremy Meyer
CEO of RoboSwap, Team Lead

Background:
Previously at Cardano, Square, AlgoWealth. 7 years of experience developing software systems at scale in consumer software and financial markets.

Social Profiles:
- https://www.linkedin.com/in/jeremypmeyer/
- https://github.com/jeremyjs

1-2 Senior Software Engineers?

TODO: William & Xoakin let's fill this out

2-4 Junior Software Engineers?

TODO: William & Xoakin let's fill this out

**Entity Information**

>Please provide the following:
>- Legal structure: Legal name, entity type, and registered address (needed for grant contract, may be shared privately)
>- Entity website link (if available)
>- Entity GitHub link (if available)

BlockRock Technologies, Inc. a Delaware Class C Corporation
(the team behind RoboSwap)

REGISTRATION PENDING

## 3. DEVELOPMENT ROADMAP

>Note: The information listed in this section will be included in the grant contract, so it is important that each deliverable is described in a clear and verifiable manner. Each milestone and the overall project is accepted as “completed” once Kadena has confirmed that all requirements are met and all features perform as described in this section.

***Overview***

>Please provide the following:
>- Roadmap Summary Table per example
>
>Roadmap Summary Table Example
>
>| Milestone   | Est. Duration | Funding      |
>| :---------- | :------------ | :------------|
>| [number]    | [days]        | [USD amount] |
>| 2           | 28 days       | $10,000      |
>| 3           | 14 days       | $5,000       |
>| **Total**   | **63 days**   | **$22,500**  |
>
>Note: A justification of funding requirements and a breakdown of expense categories (eg. effort, equipment, services) is helpful for application acceptance.

TODO

### Justification of Funding Requirements

We will work with a team of X people for Y weeks to deliver the first 3 stages of this project. Thereafter we will perform ongoing maintenance and improvements.

Roles & Compensation

TODO

The primary costs are all related to the delivery of professional software development services and project management, and we do not anticipate any other costs at this time.

***Milestones***

>For each milestone, please provide the following:
>- Milestone title
>- Milestone summary / objective
>- Deliverables Summary Table per example
>
>Deliverables Summary Table Example
>
>| Deliverable    | Title                  | Specification                    |
>| :------------- | :--------------------- | :--------------------------------|
>| [reference ID] | [title of deliverable] | [description of functionality]   |
>| B              | Activity dashboard     | Implement the ability to...      |
>| C              | Documentation          | Provide a tutorial to explain... |
>
>*Note: Each milestone must include documentation and a test suite (where applicable).*

1. Core JavaScript SDK

This represents the milestone of delivering all of the bare minimum core functionality required for the first public launch of the Kaddex SDK. We have determined this to be the following, but that is pending review and approval from the Kaddex team (technical, marketing, etc.) as a different set of functions may be required.

We will be developing a JavaScript library to be published on `npm`. It will have a name such as: `@kaddex/sdk-v1` or equivalent.

We will develop the following core methods or their equivalents:
  - createPair
  - addLiquidity
  - removeLiquidity
  - swapExactIn
  - swapExactOut
  - swap

We will utilize the `pact-lang-api` library to internally call the correct smart contract functions: https://www.npmjs.com/package/pact-lang-api.

NOTE: As part of the SDK project, we will not be developing the smart contract methods; instead, we will internally interface with them using the `pact-lang-api` library.

For technical examples of the nature of these functions, please refer to the Uniswap SDK v2 documentation and keep in mind that the specific details will depend on the Kaddex & Kadenaswap smart contract implementation.

Please refer to the relevant source for such information. Here, a link to the Kadenaswap source code is provided simply as an example:
https://github.com/kadena-io/kadenaswap/blob/master/pact/exchange.pact

| Deliverable    | Title                  | Specification                    |
| :------------- | :--------------------- | :------------------------------- |
| [reference ID] | [title of deliverable] | [description of functionality]   |
| A              | createPair             | JavaScript wrapper function      |
| B              | addLiquidity           | JavaScript wrapper function      |
| C              | removeLiquidity        | JavaScript wrapper function      |
| D              | swapExactIn            | JavaScript wrapper function      |
| E              | swapExactOut           | JavaScript wrapper function      |
| F              | swap                   | JavaScript wrapper function      |

2. Core JavaScript SDK Documentation

We will develop the core documentation to explain the concepts required for consumers to interact with the protocol. An example of the form of such background contextual and conceptual information can be found below:
https://docs.uniswap.org/protocol/V2/concepts/core-concepts/swaps

In addition, we will develop a complete and comprehensive developer documentation of the entire library, including every public function, both input parameters as well as return values, and a clear explanation of what those functions do, and how to use them for a variety of the most common use cases.

Example of a documentation page for a set of library functions:
https://docs.uniswap.org/protocol/V2/reference/smart-contracts/router-02

| Deliverable    | Title                  | Specification                                  |
| :------------- | :--------------------- | :--------------------------------------------- |
| [reference ID] | [title of deliverable] | [description of functionality]                 |
| A              | createPair             | Complete documentation for JavaScript function |
| B              | addLiquidity           | Complete documentation for JavaScript function |
| C              | removeLiquidity        | Complete documentation for JavaScript function |
| D              | swapExactIn            | Complete documentation for JavaScript function |
| E              | swapExactOut           | Complete documentation for JavaScript function |
| F              | swap                   | Complete documentation for JavaScript function |
| G              | Contextual Information | Clear, effective documentation of the core concepts and explanations of proper installation, interaction, and usage. |

3. Core TypeScript SDK

We will ensure support of TypeScript in addion to JavaScript by including the relevant type information in the library according to the most recent industry standards at the time of development.

A link to the TypeScript github project repository is included below just for reference:
https://github.com/microsoft/TypeScript

| Deliverable    | Title                  | Specification                    |
| :------------- | :--------------------- | :------------------------------- |
| [reference ID] | [title of deliverable] | [description of functionality]   |
| A              | createPair             | Comprehensive TypeScript support |
| B              | addLiquidity           | Comprehensive TypeScript support |
| C              | removeLiquidity        | Comprehensive TypeScript support |
| D              | swapExactIn            | Comprehensive TypeScript support |
| E              | swapExactOut           | Comprehensive TypeScript support |
| F              | swap                   | Comprehensive TypeScript support |

4. Auxilliary JavaScript SDK

This represents the milestone of delivering additional support for any auxilliary functions which may be developed into the exchange smart contract or any auxilliary smart contracts.

Some examples of such functions includes but is not limited to:
- getPair
- getAllPairs
- getAmountIn
- getAmountOut
- getAmountsIn
- getAmountsOut
- etc.

Please refer to the relevant sources for such information.

Here, a link to the Uniswap Router 02 documentation is provided simply as an example of some of the auxilliary functionality which may be developed in the future. There is no guarantee that all or any of the Uniswap functionality will apply to Kaddex/Kadenaswap. This is purely provided as an example reference for additional information only.
https://docs.uniswap.org/protocol/V2/reference/smart-contracts/router-02

Here, a link to the Kadenaswap source code is provided simply as an example of the existing smart contract state. There is no guarantee that this will represent the final state, nor that it will be developed or in what way. This is purely provided as an example reference for additional information only.
https://github.com/kadena-io/kadenaswap/blob/master/pact/exchange.pact

NOTE: As part of the SDK project, we will not be developing any smart contract methods; instead, we will solely be responsible for internally interfacing with them using the `pact-lang-api` library.

| Deliverable    | Title                  | Specification                    |
| :------------- | :--------------------- | :------------------------------- |
| [reference ID] | [title of deliverable] | [description of functionality]   |
| A              | getPair                | JavaScript wrapper function      |
| B              | getAllPairs            | JavaScript wrapper function      |
| C              | getAmountIn            | JavaScript wrapper function      |
| D              | getAmountOut           | JavaScript wrapper function      |
| E              | getAmountsIn           | JavaScript wrapper function      |
| F              | getAmountsOut          | JavaScript wrapper function      |

5. Auxilliary JavaScript SDK Documentation

We will develop the core documentation to explain the concepts required for consumers to interact with the protocol. An example of the form of such background contextual and conceptual information can be found below:
https://docs.uniswap.org/protocol/V2/concepts/core-concepts/swaps

In addition, we will develop a complete and comprehensive developer documentation of the entire library, including every public function, both input parameters as well as return values, and a clear explanation of what those functions do, and how to use them for a variety of the most common use cases.

Example of a documentation page for a set of library functions:
https://docs.uniswap.org/protocol/V2/reference/smart-contracts/router-02

| Deliverable    | Title                  | Specification                                  |
| :------------- | :--------------------- | :--------------------------------------------- |
| [reference ID] | [title of deliverable] | [description of functionality]                 |
| A              | getPair                | Complete documentation for JavaScript function |
| B              | getAllPairs            | Complete documentation for JavaScript function |
| C              | getAmountIn            | Complete documentation for JavaScript function |
| D              | getAmountOut           | Complete documentation for JavaScript function |
| E              | getAmountsIn           | Complete documentation for JavaScript function |
| F              | getAmountsOut          | Complete documentation for JavaScript function |

6. Auxilliary TypeScript SDK

We will ensure support of TypeScript in addion to JavaScript by including the relevant type information in the library according to the most recent industry standards at the time of development.

A link to the TypeScript github project repository is included below just for reference:
https://github.com/microsoft/TypeScript

| Deliverable    | Title                  | Specification                    |
| :------------- | :--------------------- | :------------------------------- |
| [reference ID] | [title of deliverable] | [description of functionality]   |
| A              | getPair                | Comprehensive TypeScript support |
| B              | getAllPairs            | Comprehensive TypeScript support |
| C              | getAmountIn            | Comprehensive TypeScript support |
| D              | getAmountOut           | Comprehensive TypeScript support |
| E              | getAmountsIn           | Comprehensive TypeScript support |
| F              | getAmountsOut          | Comprehensive TypeScript support |

## 4. ADDITIONAL INFORMATION

1. **Market fit:** What problem / need does your project address and how is it different from existing solutions?

We are providing the first fully comprehensive swap SDK for the Kadena ecosystem.

2. **Current progress:** Has any work been done so far? Does this project build on / rely on any existing software? Please share any relevant links and mockups.

We have not started work, and are pending approval from the Kaddex team.

3. **Engagement:** How do you plan to roll out the completed project for community awareness and engagement?

We will partner with the Kaddex team to incorporate SDK development into the public roadmap and announce the stages of completion to get early developer feedback and usage.

4. **Future plans:** Once the project is completed, do you plan to maintain or build upon it in the future?

We will partner with the Kaddex team to maintain and extend this SDK for the foreseeable future.

5. **Other:** Please share any other relevant information.

N/A
