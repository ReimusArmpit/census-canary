# Census canary rows — theodolite census

The 64 canary rows from our layer runs, exactly as the kit wrote them.

## Layer 41 (`L41-break_rel`)

`L41-break_rel.canary.jsonl` — the canary of our layer 41 run
(`L41-break_rel`).

| | |
|---|---|
| rows | 64 |
| canonical fingerprint (sha256) | `96b883ee578b2b5908cf72268e0279b84b3667f9ec35d2d32532ddf997466517` |
| card | NVIDIA GeForce RTX 5090 32 GB |
| torch / cuda | 2.14.1+cu130 / 13.0 |
| transformers | 5.20.0 |
| kit git | `041b7e4ba3d2628f2ebcb9125d2bacc0f1a5c2dd` (clean) |
| act_scale sha256 | `23a6dcefaf4eae99222c334a8294f773e37e4f20cbf36b63344a73fd5c2911fa` |
| kinds | 59 neuron, 4 random, 1 baseline |
| doses | -2: 16, -1: 16, 0: 1, +1: 16, +2: 15 |

The fingerprint is the sha256 of the rows as canonical JSON (sorted keys, no
spaces, one per line, in their order) — the same thing `census_board.py`
computes, and the same one the kit's own `L41.canary_check.json` reports.

The kit's check on this canary: *identical: 64 answers, every field* to the
home card's canary of layer 41, so this run is of the home card's class
(`bits=home`).

## Layer 47 (`L47-break_rel`)

`L47-break_rel.canary.jsonl` — the canary of our layer 47 run.

| | |
|---|---|
| rows | 64 |
| canonical fingerprint (sha256) | `d29b4c2e8fc6c6f8de781301055ca3cc370375c0d89de24a0bb5a98c0ba1b6d4` |
| card | NVIDIA RTX PRO 6000 Blackwell Server Edition (96 GB) |
| torch / cuda | 2.14.1+cu130 / 13.0 |
| transformers | 5.20.0 |
| kit git | `041b7e4ba3d2628f2ebcb9125d2bacc0f1a5c2dd` (clean) |
| act_scale sha256 | `23a6dcefaf4eae99222c334a8294f773e37e4f20cbf36b63344a73fd5c2911fa` |
| kinds | 59 neuron, 4 random, 1 baseline |
| doses | -2: 16, -1: 16, 0: 1, +1: 16, +2: 15 |

Each row carries `layer`, `kind` (`baseline` / `neuron` / `random`), `neuron`,
`prompt`, `dose`, `push`, `rel_push`, `text`, `finish`, `n_gen`, `token_ids`,
`logprob`, `top_ids` and `top_lps`.
