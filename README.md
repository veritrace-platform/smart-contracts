# smart-contracts

Solidity contracts for VeriTrace on-chain commitments. `SupplyChainTraceability` stores Merkle roots of
batched shipment events and cold-chain incidents, written only by the platform relayer.

> **Status:** planned for milestone M2 (EP5). The interface is final; implementation starts with
> `SCM-EP5-US01`.

## Design

- Interface and batch manifest format:
  [smart-contract.md](https://github.com/veritrace-platform/veritrace/blob/main/docs/contracts/smart-contract.md)
- Rationale:
  [ADR-0014](https://github.com/veritrace-platform/veritrace/blob/main/docs/adr/0014-on-chain-commitments.md)

## Toolchain

| Tool | Version |
| --- | --- |
| Solidity | 0.8.30, EVM `cancun` (pinned in `foundry.toml`) |
| Foundry | latest stable (`forge`, `cast`, `anvil`) |
| OpenZeppelin Contracts | 5.x, installed with `forge soldeer` |
| Network | Polygon Amoy (chain ID 80002) |

## Layout

```
src/        contracts
test/       Foundry unit, fuzz, and invariant tests
script/     deployment scripts
```

## License

[MIT](LICENSE)
