# quasarnova

**Model-driven OPC UA servers for industrial control — one design file, a complete server.**

You describe your device in a single XML design; a quasarnova engine turns it into a
running, standards-compliant OPC UA server. The design is the single source of truth —
address space, configuration validation and device-logic plumbing come for free, and
every engine serves the same server.

**Website: [quasarnova-team.github.io](https://quasarnova-team.github.io/)**

| Product | What it is | Status |
|---------|------------|--------|
| [kilonova](https://github.com/quasarnova-team/kilonova) | The Python engine: the same design file served in pure Python — no code generation, no compiler, live in seconds. Device simulators, test rigs, CI test doubles. [Docs](https://quasarnova-team.github.io/kilonova/) · [PyPI](https://pypi.org/project/kilonova/) | **shipping** — [![PyPI](https://img.shields.io/pypi/v/kilonova?label=pypi)](https://pypi.org/project/kilonova/) |
| [supernova](https://github.com/quasarnova-team/supernova) | The C++ engine: full model-driven framework, extended with OPC UA Pub/Sub (publisher + subscriber, UADP over UDP) on both supported OPC UA stacks. [Pub/Sub docs](https://github.com/quasarnova-team/supernova/blob/master/Documentation/source/PubSub.rst) | **released — early** [![release](https://img.shields.io/github/v/release/quasarnova-team/supernova?label=release)](https://github.com/quasarnova-team/supernova/releases/latest) |
| [hypernova](https://github.com/quasarnova-team/hypernova) | The data-interchange fabric: DIP's proven shape — named publications, a registry with a live browser, subscribe by name, boundary relays — rebuilt on OPC UA Pub/Sub. Python & Java clients. | **released — early** [![release](https://img.shields.io/github/v/release/quasarnova-team/hypernova?label=release)](https://github.com/quasarnova-team/hypernova/releases/latest) |

*Roadmap: typed client libraries (dwarfnova) and SCADA/HMI integration (rednova) are planned — no cards until they ship.*

*Heritage: quasarnova builds on the lineage of the open-source
[quasar framework](https://github.com/quasar-team/quasar) (LGPL-3.0), developed at CERN
and running large-scale control systems for more than a decade. quasarnova is an
independent project and is not affiliated with or endorsed by CERN. supernova is a fork
of quasar and preserves its copyright and license notices in full; kilonova is
conformance-tested against quasar's own public CI suite.*
