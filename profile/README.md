# BeL2

Welcome to BeL2! You're at the root of the BeL2 organization. Here are a few things you can discover here:

## Core Technology

The following services are part of the BeL2 infrastructure.

- **Cairo circuit**
  - Core technology made of cairo circuits. Used to generate and verify BTC transaction proofs.
  - https://github.com/BeL2Labs/BTCVerifier
- **EVM ZKP contract**
  - Core ZKP contract that receives requests to verify BTC transactions, and stores the list of verified transactions for other contracts to know when a transaction has been verified and its content is ready to be used on the EVM.
  - https://github.com/BeL2Labs/zkproof-demo-contracts
- **ZKP BTC Transaction Verifier**
  - EVM contract that easily allows any dApp to request verification of a BTC transaction, and get the verification status. This is a layer on top of the core ZKP contract.
  - https://github.com/BeL2Labs/BtcTxVerifier

## Loan Demo

- **React frontend**
  - React frontend app deployed at https://lending.bel2.org, that demonstrates lending USDT by locking BTC
  - https://github.com/BeL2Labs/bel2-loan-front
- **Loan contract**
  - https://github.com/BeL2Labs/Loan_Contract

## Swap Demo

- **React frontend**
  - React frontend app deployed at https://swap.bel2.org, that demonstrates EVM tokens swap against BTC in a trustless way, using BeL2 ZKP services.
  - https://github.com/BeL2Labs/bel2-swap-front
- **Swap contracts**
  - EVM contracts that handle swap orders (creation, verificatin, withdraw...). Used by the react frontennd, and use the ZKP infrastructure to verify payment transactions.
  - https://github.com/BeL2Labs/AssetExchange
  - https://github.com/BeL2Labs/TokenExchange
- **Exchange automations service**
  - This service monitors BTC payments for swap orders, and automatically generates and submits payment proofs for verification to the ZKP contracts (convenience service to avoid swap users to manually submit proofs).
  - https://github.com/BeL2Labs/bel2-exchange-automations

## Documentation

- **Gitbook**
  - Repository synchronized with BeL2 gitbook documentation.
  - https://github.com/BeL2Labs/bel2-gitbook
