# Taho challenge

## Intro

Hello talented but probably nervous human being!

We are here to get to know each other a bit better! The goal of this test is for you \
to get a quick glimpse of our daily problems, and for us to get to know you through \
code a little bit.

It's ok to not finish the whole assignment, or to cut corners. The code is important, for sure \
but the most important thing is how you think, approach problems, consider tradeoffs and \
communicate these.

We all have different level of stress tolerance, strengths and experience with blockchain tech. \
This assignment will serve as a point of discussion and is _NOT_ the final deciding factor.

Feel free to complete the tasks in any order that fits you and makes sense!

## Spec

Please fork this repo, and implement a simple single page app that

- Let's the user connect to their wallet
  - (optional) Verify if the used wallet is Taho
- Implements sign in with ethereum for signing in
- Signs an arbitrary text using the wallet and save it to local storage
  - Please choose which RPC method you want to use!
- Use alchemy api to
  - Get the token balances for the connected address
  - (optional) Get the metadata for the tokens
  - Display the output according the mockup

⚠️ Alchemy credentials

- api key `_ArbR3W9Ttz3Cx1Ofa_vVhcIxzxbx7tC`
- https endpoint: `https://eth-mainnet.g.alchemy.com/v2/_ArbR3W9Ttz3Cx1Ofa_vVhcIxzxbx7tC`

Feel free to use your own, if it's helpful.

### Wireframe

![Taho challange wireframe](wireframe.png?raw=true "Title")

### Tech requirements

- use react + typescript
- feel free to use any lib you are comfortable with

## Thought experiments / Discussion points

These questions are close to our daily work. Give them some thought and let's chat about them!

- How would you verify if the used wallet is Taho or not? How would you workaround the verification?
- Did we get all the available token balances for the user?
  - What are the upsides and downsides of the current solution? How could we mitigate downsides?
- What libs did you use and why?

## References

- [The manifest dApp that we are currently working on](https://github.com/tahowallet/taho.xyz/tree/manifesto-dapp)
- [ethers.js](https://docs.ethers.io/v5/)
  - [bignumber](https://docs.ethers.io/v5/api/utils/bignumber/)
- [EIP-1193 RPC communication standard](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1193.md)
- [Taho extension codebase](https://github.com/tahowallet/extension)
  - [our `getTokenBalances()`](https://github.com/tahowallet/extension/blob/831676b8807e61b59a99821f0cc2ba80992b8f3f/background/lib/alchemy.ts#L145)
- [Sign in with ethereum](https://login.xyz/)
  - docs + demo
- [Alchemy docs](https://docs.alchemy.com/alchemy/)
  - [alchemy_getTokenBalances](https://docs.alchemy.com/alchemy/enhanced-apis/token-api/alchemy_gettokenbalances)
  - [alchemy_gettokenmetadata](https://docs.alchemy.com/alchemy/enhanced-apis/token-api/alchemy_gettokenmetadata)
- [placehodler](https://placehodler.shapelabs.co/)

  ## Feedback

  How could we improve this test?
