# Advisories

This is a list of all ASA advisories issued by the `/security` to date:

| Advisory | Team | Severity | Title |
|----------|------|----------|----|
|[ASA-2023-001](https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-23px-mw2p-46qm) | Cosmos SDK | Medium|Cosmovisor|
|[ASA-2023-002](https://github.com/cometbft/cometbft/security/advisories/GHSA-hq58-p9mv-338c) | CometBFT | Low|Default for `BlockParams.MaxBytes` consensus parameter may increase block times and affect consensus participation|
|[ASA-2024-001](https://github.com/cometbft/cometbft/security/advisories/GHSA-qr8r-m495-7hc4) | CometBFT | High|Validation of `VoteExtensionsEnableHeight` can cause chain halt|
|[ASA-2024-002](https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-2557-x9mg-76w8) | Cosmos SDK | Medium|Default `PrepareProposalHandler` may produce invalid proposals when used with default `SenderNonceMempool`|
|[ASA-2024-003](https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-4j93-fm92-rp4m) | Cosmos SDK | Low|Missing `BlockedAddressed` Validation in Vesting Module|
|[ASA-2024-004](https://github.com/cometbft/cometbft/security/advisories/GHSA-555p-m4v6-cqxv) | CometBFT | Low|Default configuration param for Evidence may limit window of validity|
|[ASA-2024-005](https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-86h5-xcpx-cfqc) | Cosmos SDK | Low|Potential slashing evasion during re-delegation|
|[ASA-2024-006](https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-95rx-m9m5-m94v) | Cosmos SDK | High|ValidateVoteExtensions helper function may allow incorrect voting power assumptions|
