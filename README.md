# unrevealed_mint

This pseudo-standard would allow data consumers such as markets, rarity sites, tools, etc to automatically determine whether a mint is in an unrevealed state.

## Specification

Creators and launchpads can denote an unrevealed mint by appending `#h` to the on-chain metadata URI.

I.e. the metadata URI:

`https://bafybeiazvwml2lk5crhil2xr4xak52kj3yqujuuabpow7ykqq2d25ruvmm.ipfs.nftstorage.link/0.json`

Would become:

`https://bafybeiazvwml2lk5crhil2xr4xak52kj3yqujuuabpow7ykqq2d25ruvmm.ipfs.nftstorage.link/0.json#h`

## Rationale

By embedding the unrevealed state in the metadata URI, data consumers can quickly make decisions about whether to process a mint without fetching the external metadata JSON.

The marker is automatically removed once the on-chain metadata URI is updated to reveal the mint.
