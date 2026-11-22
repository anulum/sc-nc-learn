<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-LEARN — repository foundation
-->

# Architecture

## Current executable surface

The checkout contains:
- repository validation tooling;
- dedicated tests;
- workflow definitions;
- native documentation.

No domain component of SC-NC Learn is implemented yet, and no code has moved here from SC-NeuroCore. The metadata keeps domain capabilities, claims and qualified record formats empty.

## Intended records

1. **Training recipe:** How a network is trained: data, objective, schedule, seed and target format.
2. **Quantised weights:** A trained network's weights in their target numeric format, with their source.
3. **Plasticity trace:** How weights changed under a plasticity rule over a run.

## Ownership

**This project owns** the planned SC-NC Learn records and boundary rules.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| datasets and encoders | SC-NC Data |
| compilation of trained networks | SC-NC Compiler |
| model lifecycle and promotion | DIRECTOR-AI |
| the public package, documentation and releases of the monolith | SC-NeuroCore |

## Interpretation

- **Accuracy.** A figure holds only for its declared evaluation split.
- **Moves.** Code arrives only through SC-NeuroCore's split import gate, unit by unit; a planned move is not a moved capability.

Read [the documentation architecture](docs/ARCHITECTURE.md) for the planned records, rules and schema identifiers.
