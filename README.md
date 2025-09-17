# CosmicGATE-programs

CosmicGATE Program Library — Solana (Anchor) programs for node orchestration and staking rewards.

What’s inside

- orchestrator (crate: cosmicgate-sol)
    - Registers nodes (mints a soulbound NFT for each) and manages tasks (add/update).
    - Program ID (declared): 4HT4D74NjcEAdM6qbCEkmFmec2qZyVEG4njfv5oavzje
- staking-reward (crate: gate-staking-reward)
    - Staking and rewards distribution; orchestrator-level config (treasury, SOL price, base reward, slashing).
    - Program ID (declared): CKPRD8BmgaejmMBC55YzqqMDt834hSu8A2JezTxdnahM

Quick build

- Native: `cd orchestrator && anchor build` | `cd staking-reward && anchor build`
- For Solana SBF: `cd orchestrator && cargo build-sbf` | `cd staking-reward && cargo build-sbf`

Notes

- These are Anchor-based programs written in Rust.
- If you deploy new binaries, update declare_id! to match the deployed program address.

License
MIT — see LICENSE.
