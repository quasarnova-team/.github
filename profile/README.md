# quasarnova

**Model-driven OPC UA servers for industrial control — one design file, a complete server.**

You describe your device in a single XML design; a quasarnova engine turns it into a
running, standards-compliant OPC UA server. The design is the single source of truth —
address space, configuration validation and device-logic plumbing come for free, and
every engine serves the same server.

**Website: [quasarnova-team.github.io](https://quasarnova-team.github.io/)**

| Engine | What it is | Status |
|--------|------------|--------|
| [supernova](https://github.com/quasarnova-team/supernova) | The C++ engine: full model-driven framework, extended with OPC UA Pub/Sub (publisher + subscriber) on both supported OPC UA stacks. | in development |
| [kilonova](https://github.com/quasarnova-team/kilonova) | The Python engine: the same design file served in pure Python — no code generation, no compiler, live in seconds. [Docs](https://quasarnova-team.github.io/kilonova/) · [PyPI](https://pypi.org/project/kilonova/) | **shipping** — [![PyPI](https://img.shields.io/pypi/v/kilonova?label=pypi)](https://pypi.org/project/kilonova/) |
| dwarfnova | Typed client libraries generated from the same design. | planned |
| rednova | SCADA/HMI integration derived from the model. | planned |

*Heritage: quasarnova builds on the lineage of the open-source
[quasar framework](https://github.com/quasar-team/quasar) (LGPL-3.0), developed at CERN
and running large-scale control systems for more than a decade. quasarnova is an
independent project and is not affiliated with or endorsed by CERN. supernova is a fork
of quasar and preserves its copyright and license notices in full; kilonova is
conformance-tested against quasar's own public CI suite.*
