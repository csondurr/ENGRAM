# Validation record

## Evidence class

The current public package contains numerical MATLAB/full-wave-derived research outputs and figures. It does not contain an independent anechoic-chamber or over-the-air hardware validation campaign.

## Reported numerical results

- 5.800 GHz operating frequency
- 16 x 16 dual-polarized programmable aperture
- 2-bit cell-state quantization
- 25.67 dB minimum reported focus gain
- 0.03369 m² reported -3 dB focal area
- Four stored electromagnetic engrams
- 100% reported recall at a 10 dB decision threshold with 20% dropout
- 102% relative retained power after the reported 20% cell-loss experiment
- -0.89 dB reported 2-bit quantization penalty
- 18.06 dB reported median unseen-scene gain
- 91.7% reported identification accuracy

These values describe the archived computational campaign and must not be presented as independent hardware measurements.

## Reproduction boundary

The repository currently publishes the report and generated visual evidence, but not the complete executable simulation source and environment lock. Therefore it is an archival research package, not yet a fully independently reproducible software release.

## Required next validation

1. Publish or escrow the complete parameter set and executable numerical workflow.
2. Repeat the campaign from a clean environment with fixed random seeds.
3. Perform full-wave cross-validation for selected cases.
4. Build a reduced-scale aperture demonstrator.
5. Measure focus gain, recall robustness, quantization penalty, and fault tolerance independently.
