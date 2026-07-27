# ⟁ HXC 100-Cycle Novelty-Audited Math Inventor

**HyperMorphic Xenoglyphic Calculus — proof-carrying Unicode finite-mathematics discovery in one Google Colab flow**

> The representation language is part of the search space.

The **HXC 100-Cycle Novelty-Audited Math Inventor** is an executable research pipeline that repeatedly constructs finite algebraic operations, assigns them fresh Unicode notation, synthesises identities, attacks those identities with countermodels, and emits Lean 4 projects whose surviving finite claims can be checked by the Lean kernel.

The runner is contained in:

[`HXC_100_CYCLE_NOVEL_MATH_INVENTOR_COLAB`](./HXC_100_CYCLE_NOVEL_MATH_INVENTOR_COLAB)

It is designed to run as a single flowing Python script in Google Colab.

This is not merely an equation generator. Each accepted cycle must carry evidence for:

- a concrete finite operation table;
- non-degeneracy and structural dependence;
- rejection from selected known algebraic catalogues;
- isomorphism and anti-isomorphism deduplication;
- a non-seeded symbolic identity;
- a countermodel from a recognised neighbouring algebraic family;
- a separate model satisfying every advertised positive law while falsifying the identity;
- an exact equation-database audit;
- generated Lean 4 definitions, theorems and certificates;
- a source audit rejecting proof placeholders and unsafe declarations;
- successful Lean elaboration and Lake build when verification is enabled.

The system therefore implements a concrete subset of the wider HyperMorphic Xenoglyphic Calculus programme:

> **A proof-carrying Unicode finite-mathematics invention engine.**

---

## Contents

1. [What the system does](#what-the-system-does)
2. [Pipeline overview](#pipeline-overview)
3. [What V10 adds](#what-v10-adds)
4. [The mathematical search object](#the-mathematical-search-object)
5. [Novelty audit](#novelty-audit)
6. [Identity synthesis and falsification](#identity-synthesis-and-falsification)
7. [Lean 4 certification](#lean-4-certification)
8. [Default configuration](#default-configuration)
9. [Running in Google Colab](#running-in-google-colab)
10. [Configuration variables](#configuration-variables)
11. [Generated outputs](#generated-outputs)
12. [Example accepted cycle](#example-accepted-cycle)
13. [Reproducibility and resume behaviour](#reproducibility-and-resume-behaviour)
14. [Research-integrity statement](#research-integrity-statement)
15. [Limitations](#limitations)
16. [Research directions](#research-directions)
17. [Citation](#citation)
18. [Licence](#licence)

---

## What the system does

For each requested cycle, HXC attempts to produce a new proof-carrying finite algebraic candidate.

The cycle performs the following work:

1. scans the Unicode database and constructs a filtered registry of usable symbols;
2. generates or reloads complete small-order catalogues for selected algebraic families;
3. samples candidate binary-operation tables;
4. rejects degenerate, projection-like and low-information operations;
5. canonicalises each operation under every carrier relabelling;
6. also deduplicates against the opposite operation;
7. rejects structures already accepted in earlier cycles;
8. calculates algebraic laws and structural metrics;
9. assigns fresh Unicode glyphs to the structure, operation, symmetry and identity;
10. synthesises non-seeded symbolic identities that hold on the candidate;
11. tests each identity against a mixed comparison bank;
12. records countermodel results by source category rather than reporting only the first failure;
13. requires a countermodel from a loaded algebra-family catalogue;
14. searches for a model that satisfies all advertised positive laws but falsifies the identity;
15. checks for exact matches in downloaded public equation databases;
16. generates Lean 4 source for the operation, symmetry, laws, exclusions, identity and countermodels;
17. audits the Lean source for forbidden proof shortcuts;
18. asks Lean and Lake to verify the generated project;
19. stores machine-readable records, human-readable reports and proof output;
20. continues until the requested cycle count is complete or the retry budget is exhausted.

---

## Pipeline overview

```text
┌─────────────────────────────────────────────────────────────────────┐
│ 1. FILTERED UNICODE REGISTRY                                        │
│    Scan Unicode → remove unsafe/invisible/control symbols            │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 2. COMPLETE SMALL-ORDER CATALOGUES                                  │
│    Shelves · spindles · racks · quandles · kei · quasigroups         │
│    Canonical forms + hashes + cached manifests                       │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 3. FINITE-OPERATION SEARCH                                          │
│    Generate tables → score entropy/support/distance → reject trivial │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 4. ISOMORPHISM AUDIT                                                │
│    All carrier relabellings + opposite-operation deduplication       │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 5. IDENTITY SYNTHESIS                                               │
│    Generate symbolic terms → group by semantics → form identities    │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 6. ADVERSARIAL FALSIFICATION                                        │
│    References + catalogues + random holdout + law-preserving models  │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 7. DATABASE NOVELTY AUDIT                                           │
│    Alpha-canonical exact matching + explicit database-scope status   │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 8. LEAN 4 CERTIFICATION                                             │
│    Generate source → source audit → elaborate → Lake build           │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 9. PROOF-CARRYING OUTPUT                                            │
│    Reports · JSON · Lean · countermodels · hashes · packaged archive │
└─────────────────────────────────────────────────────────────────────┘
```

---

## What V10 adds

V10 strengthens the original 100-cycle inventor in several important ways.

### Category-resolved countermodels

Earlier versions could report the first countermodel encountered in an ordered model bank. That made a simple reference operation, such as a projection or modular operation, disproportionately likely to become the displayed witness.

V10 audits the full comparison bank and reports results by category:

- left and right shelves;
- left and right spindles;
- left and right racks;
- left and right quandles;
- left and right kei;
- quasigroups;
- core reference operations;
- random equivariant holdout models.

The selected catalogue countermodel is chosen from recognised neighbouring families rather than being merely the first mismatch in list order.

### Required catalogue failure

By default, an identity is rejected unless at least one loaded catalogue member falsifies it.

This raises the bar above:

> “The equation is not true of modular addition.”

The system instead requires evidence that the identity distinguishes the candidate from at least one mathematically relevant comparison family.

### Positive-law independence

Suppose a candidate operation is advertised as:

```text
left_alternative
right_alternative
surjective
```

It is not enough to show that a discovered identity holds on that candidate. The identity might simply be a consequence of those already-known laws.

V10 therefore searches for a separate finite operation that:

1. satisfies every advertised positive law; and
2. falsifies the discovered identity.

A successful witness proves a finite non-implication result:

```text
advertised positive laws ⊬ discovered identity
```

The search is tiered:

1. loaded order-4 catalogue and reference models sharing the law package;
2. law-compatible models already present in the comparison bank;
3. exhaustive order-2 and order-3 operation tables by default;
4. targeted random order-4 models respecting easy syntactic laws.

### Multiple identity rounds

Each candidate structure receives multiple identity-search rounds with deterministic seed offsets. A structure is rejected when no identity survives all required gates.

### Stronger retry behaviour

Each requested cycle can try multiple structure seeds. Failed attempts are recorded, while successful cycles are resumable.

### Exact equation-database audit

Candidate identities are alpha-canonicalised and compared against downloaded public equation lists. The system distinguishes:

- `exact_match_in_loaded_database`;
- `no_exact_match_within_loaded_database_scope`;
- `identity_exceeds_loaded_database_size_scope`;
- `novelty_databases_unavailable`.

An identity outside the operation-count scope of a database is not incorrectly labelled as a database non-match.

### Explicit historical-novelty gate

Every generated certificate preserves:

```text
historicalNoveltyVerified := false
```

unless a separate historical and literature audit is performed outside this pipeline.

---

## The mathematical search object

The default search uses a four-element carrier:

\[
A=\{0,1,2,3\}
\]

and a binary operation

\[
\star:A\times A\rightarrow A.
\]

The operation is represented by a complete table:

\[
T_{xy}=x\star y.
\]

For order four, each table contains sixteen entries.

The system searches for non-degenerate finite magmas rather than assuming associativity, commutativity, identities, inverses or distributivity.

Candidate properties include:

- commutativity;
- associativity;
- idempotence;
- flexibility;
- left alternativity;
- right alternativity;
- mediality;
- left self-distributivity;
- right self-distributivity;
- Latin or quasigroup behaviour;
- surjectivity;
- dependence on both arguments;
- non-trivial automorphism structure.

### Isomorphism

Two operations are treated as equivalent when one is obtained from the other by relabelling the carrier.

For a permutation \(\pi:A\rightarrow A\), the relabelled law is

\[
x\star_{\pi}y
=
\pi\!\left(
\pi^{-1}(x)\star\pi^{-1}(y)
\right).
\]

At order four, the system checks all \(4!=24\) relabellings.

### Anti-isomorphism

The opposite operation is

\[
x\star^{\mathrm{op}}y=y\star x.
\]

Canonicalisation is performed both on the original table and its opposite, preventing left/right mirror duplicates from being accepted as separate discoveries.

---

## Novelty audit

HXC uses a layered novelty model.

### Layer 1 — Valid finite object

The candidate is a complete deterministic binary-operation table on the selected carrier.

### Layer 2 — Non-degeneracy

The operation must survive entropy, support, projection-distance and reference-distance filters. Every row must depend on the right input, and every column must depend on the left input.

### Layer 3 — Isomorphism uniqueness

The candidate must not be isomorphic or anti-isomorphic to:

- a prior accepted cycle;
- the selected reference library;
- a loaded catalogue member in the excluded families.

### Layer 4 — Catalogue exclusion

At order four, the runner constructs complete up-to-isomorphism catalogues for:

- left and right shelves;
- left and right spindles;
- left and right racks;
- left and right quandles;
- left and right kei;
- quasigroups.

Each catalogue is hashed and recorded in a manifest.

### Layer 5 — Non-seeded identity

The identity must not be one of the built-in seed laws under variable renaming and equation-side exchange.

The seed library includes standard laws such as:

- commutativity;
- associativity;
- idempotence;
- flexibility;
- left and right alternativity;
- mediality;
- left and right self-distributivity.

### Layer 6 — Catalogue countermodel

The identity must fail on a recognised catalogue member when catalogue failure is required.

### Layer 7 — Positive-law independence

A separate finite countermodel must satisfy all advertised positive laws while falsifying the identity.

### Layer 8 — Exact database audit

The identity is alpha-canonicalised and compared with loaded public equation databases.

### Layer 9 — Lean kernel acceptance

The generated finite claims are accepted only when the Lean source elaborates and the Lake project builds successfully.

### Layer 10 — Historical novelty

Historical novelty is a separate research question.

The present pipeline does **not** prove that a structure or identity has never appeared in:

- published papers;
- books;
- theses;
- preprints;
- online databases not loaded by the runner;
- unpublished research;
- equivalent notation;
- stronger or weaker known equational theories.

The correct automatic claim is therefore:

> **Proof-carrying finite candidate with bounded computational novelty; historical novelty unverified.**

---

## Identity synthesis and falsification

The identity engine generates symbolic terms in variables

\[
x,y,z,w
\]

using the candidate operation.

Terms that evaluate to the same semantic vector over all assignments on the candidate table are grouped together. Distinct terms in the same semantic class become candidate identities.

For example:

\[
L(x,y,z,w)=R(x,y,z,w).
\]

A candidate identity is ranked using:

- failure rate on catalogue models;
- failure rate on random holdout models;
- failure rate on references;
- variable coverage;
- expression complexity;
- left/right balance;
- exact database-match status;
- availability of a positive-law independence witness.

The final identity must hold universally on the invented finite structure:

\[
\forall x,y,z,w\in A,\quad L(x,y,z,w)=R(x,y,z,w).
\]

It is then attacked across the comparison bank. V10 records the complete category profile:

```json
{
  "catalogue:left_shelves": {
    "sampled": 36,
    "failed": 20,
    "satisfied": 16
  },
  "catalogue:quasigroups": {
    "sampled": 35,
    "failed": 35,
    "satisfied": 0
  },
  "random_holdout": {
    "sampled": 279,
    "failed": 268,
    "satisfied": 11
  }
}
```

This profile is more informative than a single first-found counterexample.

---

## Lean 4 certification

Each accepted cycle produces a standalone Lean project containing the generated finite mathematics.

The generated theorem set includes proofs or certificates for claims such as:

```lean
every_row_depends_on_right_argument
every_column_depends_on_left_argument
alien_not_left_shelf
alien_not_right_shelf
alien_not_quasigroup
discovered_identity_not_in_seed_library
discovered_symbolic_identity
discovered_identity_has_catalogue_countermodel
positive_countermodel_satisfies_all_advertised_laws
positive_countermodel_falsifies_discovered_identity
discovered_identity_not_implied_by_advertised_positive_laws
symmetry_is_involution
symmetry_is_automorphism
symmetry_is_nontrivial
alien_not_isomorphic_to_modular_addition
alien_not_isomorphic_to_modular_multiplication
identityDiscoveryCertificate
noveltyCertificate
```

Many finite claims are proved with Lean's decidable computation:

```lean
by
  decide
```

This is appropriate for explicitly finite carriers: Lean checks the generated proposition by trusted reduction and decision procedures.

### Source audit

Before Lean verification, the generated source is rejected if it contains forbidden proof shortcuts or unsafe constructs, including:

```text
sorry
admit
local axiom
unsafe
```

The audit also checks for malformed or unbalanced Lean comments.

### Verification flow

```text
generate HXCNovel.lean
        ↓
source-placeholder audit
        ↓
lean --run StdPreflight.lean
        ↓
lake env lean HXCNovel.lean
        ↓
lake build
        ↓
cycle status = verified
```

A successful build proves that the generated declarations were accepted by the pinned Lean kernel and toolchain used in that run.

---

## Default configuration

```text
Version:                         V10
Cycles:                          100
Carrier order:                   4
Base seed:                       2026
Candidate samples per cycle:     25,000
Identity terms per round:        7,000
Comparison models:               480
Identity search rounds:          4
Maximum cycle retries:           20
Small-model search:              exhaustive through order 3
Order-4 random fallback:         20,000 attempts
Accepted order-4 witness cap:    2,048
Catalogue countermodel required: true
Positive-law independence:       true
Lean verification per cycle:     true
Resume mode:                     true
Packaged result archive:         true
Output root:                     /content/HXC100CycleNovelMathV10
Lean toolchain:                   leanprover/lean4:v4.33.0-rc1
```

The defaults are research-grade rather than quick-demo settings. A complete 100-cycle run can be computationally expensive.

---

## Running in Google Colab

### Method 1 — Paste into one cell

1. Open a new Google Colab notebook.
2. Open the raw contents of `HXC_100_CYCLE_NOVEL_MATH_INVENTOR_COLAB`.
3. Paste the full script into one cell.
4. Run the cell.

The script installs or reuses the required Lean environment automatically.

### Method 2 — Upload and run

Upload the script to `/content/`, then run:

```python
%run /content/HXC_100_CYCLE_NOVEL_MATH_INVENTOR_COLAB
```

The internal documentation also supports a `.py` filename such as:

```python
%run /content/HXC_100_CYCLE_NOVELTY_AUDITED_MATH_INVENTOR_COLAB_V10.py
```

### Fast smoke test

Set a smaller run before executing the script:

```python
%env HXC_CYCLES=1
%env HXC_SAMPLES=5000
%env HXC_IDENTITY_TERM_BUDGET=3000
%env HXC_MAX_CYCLE_RETRIES=5
%run /content/HXC_100_CYCLE_NOVEL_MATH_INVENTOR_COLAB
```

### Generate without Lean verification

```python
%env HXC_GENERATE_ONLY=1
%env HXC_VERIFY_EACH_CYCLE=0
%run /content/HXC_100_CYCLE_NOVEL_MATH_INVENTOR_COLAB
```

This produces candidate projects but does not classify them as Lean-verified.

---

## Configuration variables

### Core run controls

| Variable | Default | Meaning |
|---|---:|---|
| `HXC_CYCLES` | `100` | Requested accepted cycles |
| `HXC_ORDER` | `4` | Carrier order; accepted range is 3–5 |
| `HXC_SEED` | `2026` | Base deterministic seed |
| `HXC_SAMPLES` | `25000` | Candidate tables sampled per cycle |
| `HXC_OUTPUT_ROOT` | `/content/HXC100CycleNovelMathV10` | Run directory |
| `HXC_MAX_CYCLE_RETRIES` | `20` | Structure attempts per cycle |
| `HXC_RESUME` | `1` | Reuse successful cycle directories |
| `HXC_REQUIRE_ALL_CYCLES` | `1` | Raise an error when fewer than all requested cycles succeed |
| `HXC_PACKAGE_RESULTS` | `1` | Create a ZIP archive after the run |

### Candidate-quality controls

| Variable | Default | Meaning |
|---|---:|---|
| `HXC_MIN_NORMALISED_ENTROPY` | `0.90` | Minimum output-distribution entropy |
| `HXC_MIN_PROJECTION_DISTANCE` | `0.40` | Minimum distance from projection operations |
| `HXC_MIN_REFERENCE_DISTANCE` | `0.30` | Minimum distance from reference operations |
| `HXC_MIN_AVERAGE_SUPPORT` | `0.70` | Minimum average row/column support |

### Identity search

| Variable | Default | Meaning |
|---|---:|---|
| `HXC_IDENTITY_TERM_BUDGET` | `7000` | Generated terms per identity round |
| `HXC_IDENTITY_MODEL_LIMIT` | `480` | Comparison-bank size |
| `HXC_IDENTITY_PAIR_LIMIT` | `240` | Candidate identity pair cap |
| `HXC_IDENTITY_SEARCH_ROUNDS_PER_STRUCTURE` | `4` | Identity attempts for one structure |
| `HXC_IDENTITY_ROUND_SEED_STRIDE` | `7919` | Deterministic round-seed offset |
| `HXC_REQUIRE_CATALOGUE_COUNTERMODEL` | `1` | Require failure on a loaded catalogue model |
| `HXC_REQUIRE_IDENTITY_INDEPENDENCE` | `1` | Require a model satisfying all positive laws but falsifying the identity |
| `HXC_INDEPENDENCE_CANDIDATE_LIMIT` | `240` | Ranked identities considered for independence |

### Countermodel search

| Variable | Default | Meaning |
|---|---:|---|
| `HXC_SMALL_COUNTERMODEL_MAX_ORDER` | `3` | Maximum exhaustive small-model order |
| `HXC_EXHAUSTIVE_SMALL_MODEL_SEARCH` | `1` | Exhaust all models through the configured small order |
| `HXC_SMALL_MODEL_SEARCH_LIMIT` | `1024` | Cap used only when exhaustive mode is disabled |
| `HXC_ORDER4_INDEPENDENCE_RANDOM_ATTEMPTS` | `20000` | Targeted order-4 fallback attempts |
| `HXC_ORDER4_INDEPENDENCE_MODEL_LIMIT` | `2048` | Accepted law-compatible fallback models |

### Novelty databases

| Variable | Default | Meaning |
|---|---:|---|
| `HXC_DOWNLOAD_NOVELTY_DATABASES` | `1` | Download public equation lists |
| `HXC_REJECT_EXACT_DATABASE_MATCHES` | `1` | Reject exact alpha-canonical matches |
| `HXC_EXTRA_EQUATION_FILES` | empty | Comma-separated local equation files |
| `HXC_NOVELTY_DATABASE_CACHE` | `/content/.cache/hxc_novelty_databases` | Database cache |

### Lean and output

| Variable | Default | Meaning |
|---|---:|---|
| `HXC_LEAN_TOOLCHAIN` | `leanprover/lean4:v4.33.0-rc1` | Pinned toolchain |
| `HXC_VERIFY_EACH_CYCLE` | `1` | Run Lean verification after each accepted cycle |
| `HXC_GENERATE_ONLY` | unset | Skip Lean installation and verification when true |
| `HXC_PRINT_PROOFS` | `1` | Print selected Lean declarations |
| `HXC_PRINT_FULL_LEAN` | `0` | Print the complete generated Lean file |
| `HXC_RUN_EXTERNAL_PROVERS` | `0` | Optionally run supported external prover workflow |
| `HXC_CATALOGUE_CACHE` | `/content/.cache/hxc_catalogues` | Generated catalogue cache |

### Order note

The runner accepts orders 3–5, but complete generated shelf/quasigroup-family catalogues are implemented only through order four. At higher orders, the bounded catalogue-novelty claim is correspondingly weaker.

---

## Generated outputs

A default run writes to:

```text
/content/HXC100CycleNovelMathV10/
```

Typical layout:

```text
HXC100CycleNovelMathV10/
├── cycle_001/
│   ├── HXCNovel.lean
│   ├── StdPreflight.lean
│   ├── lakefile.toml
│   ├── lean-toolchain
│   ├── NOVEL_STRUCTURE_REPORT.md
│   ├── novel_structure.json
│   ├── catalogue_manifest.json
│   ├── identity_discovery.json
│   ├── NOVELTY_AUDIT.json
│   ├── NOVELTY_SEARCH_QUERIES.txt
│   ├── prover9_positive_laws_to_identity.in
│   ├── mace4_positive_laws_to_identity.in
│   ├── cycle_unicode.json
│   ├── LEAN_PROOF_OUTPUT.txt
│   └── cycle_status.json
│
├── cycle_002/
├── cycle_003/
├── ...
│
├── shared/
│   ├── unicode_glyph_registry.json
│   ├── catalogue_manifest.json
│   └── catalogues/
│       ├── left_shelves_order_4.json
│       ├── right_shelves_order_4.json
│       ├── quasigroups_order_4.json
│       └── ...
│
├── run_manifest.json
├── ALL_DISCOVERIES.md
├── ALL_IDENTITIES.json
└── ALL_LEAN_PROOFS.txt
```

When result packaging is enabled, the runner creates:

```text
/content/HXC100CycleNovelMathV10.zip
```

### Important files

| File | Purpose |
|---|---|
| `HXCNovel.lean` | Generated formal definitions, theorems and certificates |
| `NOVEL_STRUCTURE_REPORT.md` | Human-readable cycle report |
| `novel_structure.json` | Complete machine-readable structure record |
| `identity_discovery.json` | Identity, countermodels and novelty metadata |
| `NOVELTY_AUDIT.json` | Condensed novelty and independence audit |
| `catalogue_manifest.json` | Catalogue scope, counts and hashes |
| `LEAN_PROOF_OUTPUT.txt` | Printed proof declarations for the cycle |
| `cycle_status.json` | Seed, attempt, hashes and verification status |
| `ALL_DISCOVERIES.md` | Aggregated human-readable run summary |
| `ALL_IDENTITIES.json` | Aggregated identities and glyph assignments |
| `ALL_LEAN_PROOFS.txt` | Combined generated proof output |
| `run_manifest.json` | Complete run-level manifest |

---

## Example accepted cycle

One V10 cycle produced the following four-element operation.

### Unicode assignment

```text
Structure glyph: ⚖
Operation glyph: ⎬
Symmetry glyph:  🀒
Identity glyph:  ⥽
```

### Operation table

```text
1 2 0 0
2 0 1 1
0 1 2 3
3 3 2 3
```

### Verified positive laws

```text
left_alternative
right_alternative
surjective
```

### Synthesised identity

\[
\begin{aligned}
&((x\mathbin{\text{⎬}}(y\mathbin{\text{⎬}}x))
 \mathbin{\text{⎬}}
 ((y\mathbin{\text{⎬}}y)\mathbin{\text{⎬}}(x\mathbin{\text{⎬}}x)))\\
={}&(((x\mathbin{\text{⎬}}z)\mathbin{\text{⎬}}z)
 \mathbin{\text{⎬}}
 ((z\mathbin{\text{⎬}}x)\mathbin{\text{⎬}}(x\mathbin{\text{⎬}}x))).
\end{aligned}
\]

The run reported:

```text
Comparison failures:              439 / 480
Catalogue countermodel:           left shelf
Positive-law countermodel order:  4
Database status:                  identity exceeds loaded database size scope
Lean source audit:                passed
Lean project build:               passed
Historical novelty:               unverified
```

What this establishes is bounded but real:

- the equation holds for every assignment on the generated four-element operation;
- it is not simply one of the seeded identities;
- it fails on loaded neighbouring catalogue structures;
- it is not implied by the listed positive laws, because a separate law-preserving countermodel falsifies it;
- the finite claims were accepted by Lean.

What it does **not** establish is that the identity has never previously appeared in mathematical literature under any equivalent formulation.

---

## Reproducibility and resume behaviour

### Deterministic seeds

The run uses a base seed and deterministic offsets for:

- cycle number;
- retry number;
- identity-search round.

With the same source, environment, catalogue state and configuration, the same seed path is intended to reproduce the same candidate sequence.

### Cross-cycle deduplication

Successful cycles contribute to run-level exclusion sets containing:

- canonical operation forms up to opposite;
- canonical identity codes;
- assigned Unicode symbols.

Later cycles cannot silently reuse an earlier accepted result.

### Resume mode

With:

```text
HXC_RESUME=1
```

the runner scans existing cycle directories. A cycle is resumed only when its status and generated records indicate a previously successful `verified` or `generated` result.

Successful prior cycles are skipped, while missing cycles continue.

### Failure handling

A cycle can reject multiple candidate structures before succeeding. Rejection is expected when:

- no structure passes the novelty and quality gates;
- no identity survives catalogue and database gates;
- no positive-law independence witness is found;
- generated Lean fails to elaborate;
- the cycle exhausts its retry budget.

Failed attempts are recorded rather than hidden.

---

## Research-integrity statement

HXC distinguishes four claim levels.

### Claim A — Generated object

The program produced a complete finite operation table and associated records.

### Claim B — Verified finite property

A property or identity was exhaustively checked or formally accepted for that exact finite object.

### Claim C — Bounded computational novelty

The candidate was not equivalent to prior accepted cycles, selected references or the explicitly loaded catalogue/database scope.

### Claim D — Historically unknown mathematics

The structure, identity or theorem has never appeared anywhere in the mathematical record, including equivalent notation and stronger theories.

The current pipeline supports Claims A and B and bounded forms of Claim C.

It does not automatically establish Claim D.

This distinction is encoded directly in generated records:

```text
historicalNoveltyVerified := false
```

The project prioritises:

- reproducibility over spectacle;
- explicit search scope over vague novelty claims;
- countermodels over confirmation alone;
- semantic independence over syntactic difference alone;
- kernel checking over unsupported proof claims;
- exact hashes and manifests over unverifiable summaries.

---

## Limitations

### Historical novelty is not automated

Exact database matching is not a literature review. A candidate may be known under different variable names, notation, duality, derived laws or a stronger equational basis.

### Database comparison is exact, not semantic

The current audit checks alpha-canonical exact equality of equations. It does not prove non-equivalence under arbitrary theorem derivation.

### Finite novelty does not imply mathematical importance

A true identity on one small finite magma may be structurally interesting, accidental or highly specialised. Human mathematical interpretation remains necessary.

### The search is not exhaustive over all order-4 magmas

The default system samples candidate structures. It exhaustively handles selected subproblems, such as relabellings and small countermodel spaces, but does not enumerate every possible four-element binary operation as the main discovery search.

### Catalogue completeness is scoped

The generated catalogues are complete for the named families and supported order, not for every possible class of finite algebra.

### `by decide` is a finite proof, not an explanatory proof

Kernel-checked finite computation establishes truth for the encoded object, but it may not reveal a conceptual reason or general theorem.

### Unicode is notation, not meaning by itself

A fresh glyph names the generated operation. Mathematical significance comes from the operation table, laws, identities, countermodels and proofs—not from visual novelty.

### Runtime can be substantial

A full 100-cycle run performs repeated finite search, catalogue work, identity synthesis, countermodel testing, source generation and Lean builds.

---

## Research directions

The present engine creates proof-carrying finite candidates. Natural next steps include:

1. semantic equivalence checking against equational-theory databases;
2. integration with Prover9, Mace4 and other automated theorem tools;
3. extraction of shorter human-readable axiom bases;
4. search for identities that define non-trivial varieties rather than single structures;
5. enumeration of all models satisfying a discovered identity at small orders;
6. implication lattices among generated identities;
7. independent replication of catalogue counts and hashes;
8. literature-search tooling using canonical equation forms and algebraic keywords;
9. generalisation from one binary operation to multi-operation signatures;
10. typed HXC glyph invention linked to executable semantics;
11. invariant-aware rewriting and recoverable representation transport;
12. theorem discovery whose value survives removal of the HyperMorphic interpretation.

A particularly important upgrade would separate:

```text
finite candidate generation
        ↓
semantic theorem equivalence
        ↓
prior-art search
        ↓
expert mathematical interpretation
        ↓
historical novelty decision
```

---

## Citation

```bibtex
@software{paul2026hxc100cycle,
  author = {Shaun Paul},
  title = {HXC 100-Cycle Novelty-Audited Math Inventor},
  year = {2026},
  note = {A proof-carrying Unicode finite-algebra discovery pipeline with
          isomorphism-aware structure search, identity synthesis,
          category-resolved countermodels, positive-law independence
          witnesses, equation-database auditing, and Lean 4 certification},
  repository = {HyperMorphic-Xenoglyphic-Calculus}
}
```

Project-level citation:

```bibtex
@software{paul2026hxc,
  author = {Shaun Paul},
  title = {HyperMorphic Xenoglyphic Calculus:
           Proof-Carrying Unicode Mathematics Invention},
  year = {2026},
  note = {An experimental extensible symbolic calculus and finite-algebra
          discovery pipeline with automated conjecture generation,
          countermodel search, Unicode glyph assignment,
          and Lean 4 certification}
}
```

---

## Licence

MIT Licence.

---

## Closing expression

\[
\boxed{
\begin{aligned}
\text{finite search}
&\;\text{⟜}_{\mathrm{canonicalisation}}\;
\text{non-degenerate structure}\\
&\;\text{⟜}_{\mathrm{glyph\ invention}}\;
\text{named operation}\\
&\;\text{⟜}_{\mathrm{identity\ synthesis}}\;
\text{candidate theorem}\\
&\;\text{⟜}_{\mathrm{countermodel\ attack}}\;
\text{independent survivor}\\
&\;\text{⟜}_{\mathrm{Lean}}\;
\text{proof-carrying Xenoglyphic mathematics}.
\end{aligned}
}
\]

**The alphabet is extensible. The search is adversarial. The novelty claim is scoped. The surviving finite mathematics carries proof.**

