<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-LEARN — repository foundation
-->

# Repository architecture

## Current executable tooling

**What it contains:** the repository's metadata, source-provenance, workflow, dependency-alignment, documentation, inventory and preflight controls.

**What each control does:** it inspects its fixed, declared local scope.

**What received metadata cannot do:** select another acceptance policy or grant domain authority.

Foundation qualification is in progress.

## Intended domain boundaries

| Record | Responsibility | Required evidence |
| --- | --- | --- |
| Training recipe | How a network is trained: data, objective, schedule, seed and target format | Training reproduced from the recipe and seed on the same data |
| Quantised weights | A trained network's weights in their target numeric format, with their source | Accuracy loss from quantisation measured on a declared evaluation split |
| Plasticity trace | How weights changed under a plasticity rule over a run | Trace checks against the rule and the run |

## Planned record schemas

- `sc_nc_learn.training_recipe.v1`
- `sc_nc_learn.quantised_weights.v1`
- `sc_nc_learn.plasticity_trace.v1`

These are planned identifiers. None of them is registered or qualified here.

It also takes over, unchanged, sc-neurocore.spiking-artefact-contract (v1 and v2) from SC-NeuroCore when their code moves here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
