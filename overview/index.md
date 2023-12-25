# About

In `Mind-in-Vitro (MiV)`, we aim to develop living neuromorphic computation framework.
For more information on Mind *in Vitro*, see the project [website](https://mindinvitro.illinois.edu).

```{mermaid}
flowchart LR
    A{Analysis}
    E([Simulator])
    H([Hardware])
    R[Reservoir</br>Computing]
    C[Assembly</br>Calculus]
    D[(DB)]
    I[Interface]
    subgraph Workflow
        direction LR
        subgraph Data Collection
            H --> D
            E --> D
        end
        subgraph Open Software
            D <-->|HDF5| A
            I
        end
        subgraph Computation
            A --> R
            A --> C
        end
    end
```

## Projects

| Name                | Planed  | Description                                                       | Repo                                                  | Current Status |
| :-----------------: | :-----: | ----------------------------------------------------------------- | :--------------------------------------------:        | :------------: |
| Open Software (OS)  |         | Neuro-electrophysiology analysis and processing tools             | [public](https://github.com/GazzolaLab/MiV-OS)        | Open Source    |
| Open Hardware (OH)  |         | Electrophysiology open hardware project with design and protocols | [public](https://gazzolalab.github.io/MiV-OH)         | Open Source    |
| Interface           | 2022 Q2 | Web-based interactive GUI for spike analysis                      | private                                               | In progress    |
| Simulator           |         | Bio-realistic neurophysiology emulator using Neuron               | [public](https://github.com/GazzolaLab/MiV-Simulator) | Open Source    |
| Reservoir Computing | 2022 Q4 | Reservoir computing module for neuromorphic hardware/emulator     |                                                       |                |

> The software is developed and maintained by the Gazzola Lab at the University of Illinois at Urbana-Champaign. For more information on the projects and what we work on, visit our [website](https://mattia-lab.com).

## Contribution

Any contribution to this project is welcome! If you are interested or have any questions, please don't hesitate to contact us.
In general, we follow typical git-workflow. We prepared detailed contribution guideline [here](https://github.com/GazzolaLab/MiV-OS/blob/main/CONTRIBUTING.md).

```{toctree}
:maxdepth: 2
:caption: Overview

references
Contribution <https://github.com/GazzolaLab/MiV-OS/blob/main/CONTRIBUTING.md>
```

```{toctree}
:maxdepth: 2
:caption: Background

literature
```
