# ENGRAM

**Electromagnetic associative memory implemented with a programmable dual-polarized aperture.**

ENGRAM investigates whether a reconfigurable electromagnetic surface can learn, store, recall, and distinguish field configurations in the same operational language used by associative memory systems. The archived study operates at **5.8 GHz** with a **16 x 16 dual-polarized**, **2-bit** programmable aperture.

> **Validation status:** computational research package. The reported values are numerical/simulation results, not independent hardware measurements.

## Research objective

The project maps electromagnetic scenes to programmable aperture states and evaluates four capabilities:

- near-field focusing and scene-dependent field reconstruction;
- storage and recall of multiple electromagnetic engrams;
- robustness to cell dropout, damage, quantization, and scene change;
- discrimination between stored and previously unseen field configurations.

## System model

The aperture contains 256 dual-polarized cells. Each cell is constrained to four phase states. A channel/scene response is combined with the programmable aperture response to generate a field at the observation region. The stored configuration acts as the electromagnetic memory state. Recall is evaluated by applying disturbed or incomplete conditions and measuring whether the intended field configuration is recovered.

## Archived results

| Metric | Reported value |
|---|---:|
| Operating frequency | 5.800 GHz |
| Aperture | 16 x 16, dual polarization |
| State resolution | 2 bit |
| Minimum focus gain | 25.67 dB |
| -3 dB focal area | 0.03369 m² |
| Stored engrams | 4 |
| Recall at 10 dB threshold and 20% dropout | 100% |
| Relative power after 20% cell loss | 102% |
| Quantization penalty | -0.89 dB |
| Median unseen-scene gain | 18.06 dB |
| Identification accuracy | 91.7% |

The apparent value above 100% in the cell-loss experiment is a normalized numerical outcome and does not imply energy creation; disturbance can change constructive and destructive field addition at the selected observation point.

## Evidence map

The numbered PNG files under `results/figures/` form the visual validation sequence:

1. aperture geometry and reference phase;
2. multipath scene and channel magnitude;
3. learning convergence and near-field focus;
4. far-field response, capacity, and crosstalk;
5. associative recall and damage response;
6. quantization, Monte Carlo tolerance, and adversarial cases;
7. scene-change recovery and validation statistics;
8. full-wave element geometry, S-parameters, and pattern;
9. off-grid localization statistics.

The complete formatted archive is available as [ENGRAM.pdf](docs/ENGRAM.pdf) and [ENGRAM.html](docs/ENGRAM.html).

## Repository structure

```text
.
├── README.md
├── docs/ENGRAM.pdf
├── docs/ENGRAM.html
├── results/figures/01_...png through 20_...png
├── docs/
│   └── VALIDATION.md
├── CITATION.cff
├── CONTRIBUTING.md
├── SECURITY.md
└── LICENSE
```

## Limitations

- The public repository does not currently include the complete executable simulation source.
- The results have not yet been independently reproduced from a clean environment.
- The aperture-level claims have not yet been verified on fabricated hardware.
- Reported classification and recall metrics apply only to the archived numerical protocol.
- Performance outside the evaluated frequency, scene distribution, tolerances, and fault model is not established.

See [docs/VALIDATION.md](docs/VALIDATION.md) for the evidence boundary and required next experiments.

## Citation

Citation metadata is provided in [CITATION.cff](CITATION.cff).

## License

Copyright (c) 2026 Cem Sondur. Distributed under the [MIT License](LICENSE). The license does not convert third-party material, if any, into MIT-licensed content.
