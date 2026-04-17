# Foundation IPFS CIDs

A dataset of IPFS content identifiers (CIDs) extracted from NFT token metadata across Foundation collections on Ethereum.

## Data

`token_cids.csv` contains 343,194 tokens with the following columns:

| Column | Description |
|---|---|
| `collection` | Contract address of the NFT collection |
| `creator` | Address of the collection creator |
| `token_id` | Token ID within the collection |
| `metadata_cid` | IPFS CID of the token metadata JSON |
| `image_cid` | IPFS CID of the token image |
| `animation_cid` | IPFS CID of the token animation (if applicable) |

All CIDs are extracted from on-chain `tokenURI`, `image`, and `animation_url` fields that resolve to `ipfs://` URIs.

## Usage

Access any CID via an IPFS gateway:

```
https://ipfs.io/ipfs/{cid}
```

Or directly via IPFS:

```
ipfs:///{cid}
```

## License

This dataset is derived from public on-chain data. Released under [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
