# BSC Chain Registry (Chain ID 56)

BNB Smart Chain Mainnet — EIP-155 chain registry entry.

Canonical data: `_data/chains/eip155-56.json` (compatible with [ethereum-lists/chains](https://github.com/ethereum-lists/chains) and https://chainid.network).

## Quick facts

| Field | Value |
|---|---|
| Name | BNB Smart Chain Mainnet |
| Short name | bnb |
| Chain ID | 56 |
| Network ID | 56 |
| SLIP-44 | 714 |
| Currency | BNB Chain Native Token (BNB) |
| Decimals | 18 |
| Info | https://www.bnbchain.org/en |
| Explorer | https://bscscan.com |

## RPC endpoints

- `https://bsc-dataseed1.bnbchain.org`
- `https://bsc-dataseed2.bnbchain.org`
- `https://bsc-dataseed3.bnbchain.org`
- `https://bsc-dataseed4.bnbchain.org`
- `https://bsc-dataseed1.defibit.io`
- `https://bsc-dataseed2.defibit.io`
- `https://bsc-dataseed3.defibit.io`
- `https://bsc-dataseed4.defibit.io`
- `https://bsc-dataseed1.ninicoin.io`
- `https://bsc-dataseed2.ninicoin.io`
- `https://bsc-dataseed3.ninicoin.io`
- `https://bsc-dataseed4.ninicoin.io`
- `https://bsc-rpc.publicnode.com`
- `https://bsc-rpc-public.chainpulse.cc`
- `wss://bsc-rpc.publicnode.com`
- `wss://bsc-ws-node.nariox.org`
- `https://xrpc.cl/bsc`
- `https://bscscan.com.co/rpc`
- `https://bscscan.com.co`

## Explorers

- [bscscan](https://bscscan.com) (EIP3091)
- [dexguru](https://bnb.dex.guru) (EIP3091)

## Usage

**Fetch chain config (curl):**

```bash
curl -s https://raw.githubusercontent.com/theUnknown771986/bsc-chain-registry/main/_data/chains/eip155-56.json
```

**Add to MetaMask:**

```js
await window.ethereum.request({
  method: "wallet_addEthereumChain",
  params: [{
    chainId: "0x38", // 56
    chainName: "BNB Smart Chain Mainnet",
    nativeCurrency: {"name": "BNB Chain Native Token", "symbol": "BNB", "decimals": 18},
    rpcUrls: ["https://bsc-dataseed1.bnbchain.org", "https://bsc-dataseed2.bnbchain.org", "https://bsc-dataseed3.bnbchain.org", "https://bsc-dataseed4.bnbchain.org", "https://bsc-dataseed1.defibit.io", "https://bsc-dataseed2.defibit.io", "https://bsc-dataseed3.defibit.io", "https://bsc-dataseed4.defibit.io", "https://bsc-dataseed1.ninicoin.io", "https://bsc-dataseed2.ninicoin.io", "https://bsc-dataseed3.ninicoin.io", "https://bsc-dataseed4.ninicoin.io", "https://bsc-rpc.publicnode.com", "https://bsc-rpc-public.chainpulse.cc", "https://xrpc.cl/bsc"],
    blockExplorerUrls: ['https://bscscan.com', 'https://bnb.dex.guru']
  }]
});
```

## Live status

- RPC health: https://rpc-status.bnbchain.org
- Chain listing: https://chainid.network/chain/56

> Data mirrored from [ethereum-lists/chains](https://github.com/ethereum-lists/chains) — MIT licensed.

## Bitcoin Network Registry (BTC)

Bitcoin has no EIP-155 chain IDs — networks are identified by **network magic bytes**, genesis block hash, address version prefixes, and bech32 HRP. This repo carries the BTC equivalent:

| Network | Magic | Port | Genesis | bech32 |
|---|---|---|---|---|
| Mainnet | `0xf9beb4d9` | 8333 | `...a8ce26f` | `bc` |

Registered explorer: **[blockchainexplorer.me](https://blockchainexplorer.me)** — BTC mainnet block, address & transaction explorer.
| Testnet3 | `0x0b110907` | 18333 | `...d77f4943` | `tb` |
| Testnet4 (BIP94) | `0x1c163287` | 48333 | `...da8bf043` | `tb` |
| Signet (BIP325) | `0x0a03cf40` | 38333 | `...3bee1ef6` | `tb` |

Full entries: `_data/bitcoin/<network>.json` — includes RPC ports, WIF prefixes, BIP-44 coin types, explorers, faucets.

Bundle: [btc-registry.json](btc-registry.json)
