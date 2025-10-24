# BooCoin

A minimal Clarity smart contract project for the BooCoin fungible token.

- Contract and Clarinet project live in `clarinet/`
- Quick start:
  - Install Clarinet: https://docs.hiro.so/clarinet/getting-started/installation
  - Change into the project directory:
    - On Windows PowerShell: `cd clarinet`
  - Validate contracts: `clarinet check`
  - Open REPL: `clarinet console`

In the console you can:
- Initialize owner (once): `(contract-call? .boocoin init '<YOUR-PRINCIPAL>)`
- Mint (owner only): `(contract-call? .boocoin mint '<RECIPIENT-PRINCIPAL> u1000)`
- Transfer: `(contract-call? .boocoin transfer '<RECIPIENT-PRINCIPAL> u250)`
- Read data: `(contract-call? .boocoin get-total-supply)`, `(contract-call? .boocoin balance-of '<PRINCIPAL>)`

Note: Current contract is a minimal token and not a full SIP-010 implementation. If you want SIP-010 compliance, say "make it SIP-010" and I’ll upgrade the contract.
