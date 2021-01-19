# Drizzle, Next, Typescript and Chakra UI Truffle Box

This also includes prettier support for solidity and a greeter contract.

## Setup

<!-- TODO: truffle ubox command -->

Run the following:
`npm install`
`truffle compile`
`truffle migrate`
`npm run dev`

## How This Was Made

This is everything I did to get this setup

1. `npx create-next-app --example with-chakra-ui-typescript`
2. `truffle init`
3. delete _test_ folder
4. Change _truffle-config.js_:
   1. Add `contracts_build_directory: "./src/artifacts/",`
   2. Uncomment the development network and change the port to `7545`
5. change `build` script in _package.json_ to `next build && next export`
6. `npm install --save-dev prettier prettier-plugin-solidity`
7. `npm install @drizzle/store @drizzle/react-plugin @drizzle/react-components`
8. Changed/added a bunch of the default example files
9. `npm install @truffle/hdwallet-provider dotenv`
10. Add xDai support
