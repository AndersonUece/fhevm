# Security Considerations

This document highlights common security concerns when developing
and deploying FHEVM smart contracts.

## Private data handling

- Treat encrypted inputs and outputs as sensitive.
- Never log private keys or secret parameters.
- Minimize exposure of unencrypted values on-chain.

## Upgradability

- Use a proxy pattern carefully and document upgrade paths.
- Restrict upgrade functions to authorized accounts via multi-sig.
- Test upgrades on test networks before mainnet deployments.

## Audits and testing

- Perform static analysis with tools like Slither and MythX.
- Review zero-knowledge circuits and encryption schemes.
- Require external security audits before mainnet deployment.

By incorporating these considerations early, you reduce the risk of
security vulnerabilities in FHEVM-based applications.
