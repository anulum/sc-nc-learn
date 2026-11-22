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

SC-NC Learn is being built as the training layer split out of SC-NeuroCore, for spiking networks that run on neuromorphic hardware: training recipes, quantised weights, plasticity traces, conversion from other networks, and the spiking artefact contract that carries a trained network onward. It is distinct from Circuit Learning, which studies circuit design processes. It imports SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data and SC-NC Compiler. Its current executable surface is repository validation tooling. It has no installed trainer, quantiser, plasticity recorder or qualified record schema.

Read [Architecture](ARCHITECTURE.md), [validation tooling](validation-tooling.md), [data boundaries](THREAT_MODEL.md) and the [repository boundary decision](adr/0001-repository-boundary.md).
