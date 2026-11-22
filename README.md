<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-LEARN — repository foundation
-->

# SC-NC Learn

SC-NC Learn is being built as the training layer split out of SC-NeuroCore, for spiking networks that run on neuromorphic hardware: training recipes, quantised weights, plasticity traces, conversion from other networks, and the spiking artefact contract that carries a trained network onward. It is distinct from Circuit Learning, which studies circuit design processes. It imports SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data and SC-NC Compiler. This checkout contains repository validation tooling and documentation only. Full foundation qualification is in progress. There is no installed trainer, quantiser, plasticity recorder or qualified record schema.

**What does not exist yet:**
- any code moved from SC-NeuroCore;
- a registered runtime record schema;
- an installed trainer, quantiser or plasticity recorder.

## Boundary

**What this project owns:**

| Record | Scope |
|---|---|
| Training recipe | How a network is trained: data, objective, schedule, seed and target format |
| Quantised weights | A trained network's weights in their target numeric format, with their source |
| Plasticity trace | How weights changed under a plasticity rule over a run |

**Schemas it takes over from SC-NeuroCore:** sc-neurocore.spiking-artefact-contract (v1 and v2).

**Static imports:** only SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data and SC-NC Compiler.

**Records read without importing their code:** Model Provenance Pack, SC-NC Compiler, SC-NC Bridges, Plasticity Witness, Spike Calibrator, Deploy Pack and DIRECTOR-AI read this repository's records.

**Records it reads without importing their code:** those of SC-NC Catalogue, SC-NC Data, SC-NC Compiler and Spike Quality Gate.

**Code planned to move here from SC-NeuroCore,** package by package, when SC-NeuroCore's split import gate allows it: `learning`, `training`, `conversion`, `qat`, `nas`, `online_learning`, `continual`, `contrastive`, `distillation`, `few_shot`, `homeostasis`, `meta_plasticity`, `transfer`, `digital_twin`, `federated`, `privacy` and `spike_norm`.

**Explicit non-claims and operating boundaries:**
- No model has been trained, quantised or deployed by this foundation.
- A training recipe describes how a network was trained; it is not a claim about the network's accuracy beyond its evaluation.

## Current tooling

Repository controls inspect:
- metadata and source attribution;
- workflows and dependency alignment;
- native documentation and repository inventory;
- preflight orchestration.

Metadata declares architecture-only maturity with empty implemented domain capability and claim inventories.

- Use the exact environment in [Contributing](CONTRIBUTING.md).
- Full CI and preflight belong in CI or in an explicitly admitted pre-push environment.
- See [Validation](VALIDATION.md) for the maintained validation scope.

## Intended evidence

Every future record will carry its source and environment digests, its numeric formats where it has them, and its explicit verification boundary. None of the planned record schemas is registered or qualified by this foundation.

## Documentation and support

Read [Architecture](ARCHITECTURE.md), [support](SUPPORT.md), [security reporting](SECURITY.md) and [citation metadata](CITATION.cff).

**Not claimed:**
- a hosted service, released package or DOI;
- a public CI status;
- a performed simulation, hardware measurement or benchmark result.

## Licence

Source is licensed under [AGPL-3.0-or-later](LICENSE). A commercial licence is available through the contact in [NOTICE](NOTICE.md).

![ANULUM](docs/assets/anulum_logo_company.jpg)

![Fortis Studio](docs/assets/fortis_studio_logo.jpg)

## Text and data mining reservation
The rightsholder, Miroslav Šotek (ANULUM), expressly reserves the use of the
works in this repository for text and data mining, including the collection of
this content for, and its use in, training, fine-tuning or evaluating machine
learning and artificial intelligence models, in accordance with Article 4(3) of
Directive (EU) 2019/790 and the national provisions transposing it.

No permission for such use has been granted beyond what the licence in
`LICENSE` grants. This reservation does not change that licence: uses the
licence permits remain permitted on its terms, including its attribution and
share-alike conditions.

Reservation made on 2026-11-22. Requests for permission: contact the
rightsholder through the contact listed in this repository.
