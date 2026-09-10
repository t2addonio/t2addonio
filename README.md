# Residual streams as an addressing problem

One research line. Four public repositories.

**Grokking → causal residual isolation → distributed / additive representations → cross-domain residual addressing → real-world signal experiments.**

A researcher landing here should not have to reconstruct that order from four disconnected READMEs. The code already tells this story; the profile now does too.

## The pipeline

| Stage | What it answers | Repository |
|------|-----------------|------------|
| **1. Grokking** | After generalization, is there a residual-stream component that is *causally necessary* and distinct from known algorithmic features? | [`residual-stream-grokking`](https://github.com/t2addonio/residual-stream-grokking) |
| **2. Isolation + additive structure** | Is that component a single direction, or a set of nearly-disjoint tributaries that add? Isolate, rescue, freeze-at-transition, WD ablation. | [`isolate-rescue-grokking`](https://github.com/t2addonio/isolate-rescue-grokking) |
| **3. Cross-domain addressing** | Can the same extract / path-patch / store / read protocol address a residual on optical, RF, NV, CMB, EEG, telemetry, audio, and transformer buses? | [`residual-causal-toolkit`](https://github.com/t2addonio/residual-causal-toolkit) |
| **4. Real-world signal experiments** | Same addressing idea on live RF, edge hardware, and a human-gated multi-agent lab. No autonomous writes. | [`hybrid-lab`](https://github.com/t2addonio/hybrid-lab) |

Read them in that order. 1 is the claim. 2 is the geometry of the claim. 3 is the protocol that travels. 4 is the plant.

## One-line claim

A residual in an additive mixture can be contrastively extracted, shown load-bearing under causal intervention, and addressed on a bus that is not overwritten — in grokked transformers first, then on physical signal paths.

## How to read the code

1. Start in `residual-stream-grokking` with the paper PDF and `run_discovery_*.py` / `analyze_*.py`.
2. Then `isolate-rescue-grokking/kits/` for 16-seed isolate/rescue/phase/freeze and the additive-tributary result (`keep_only` collapse, near-additive logit deltas, disjoint fail sets).
3. Then `residual-causal-toolkit` protocol steps 1–5 (extract → filter → store/phase/beam → read) and the unified paper under `docs/papers/`.
4. Then `hybrid-lab/rf_residual_stream` plus the Coordinator/Gate if you care how the same work is operated locally.

Large checkpoints and campaign figures stay in the working store and are catalogued in each repo `INDEX.md`. Scripts regenerate what git does not hold.

## Contact

Tony Taddonio · mechanistic interpretability / residual-stream causality / live RF and audio signal paths
