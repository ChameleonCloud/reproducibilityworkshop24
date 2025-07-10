---
title: "Experiment Packaging Checklist"
source: "Report on Challenges of Practical Reproducibility for Systems and HPC Computer Science"
author: "Keahey, Kate; Richardson, Marc; Calasanz, Rafael Tolosana; Hunold, Sascha; Lofstead, Jay; Malik, Tanu; Perez, Christian"
date: "2025-04-30"
doi: "10.5281/zenodo.15306610"
---

# Appendix A: Experiment Packaging Checklist

*From [Report on Challenges of Practical Reproducibility for Systems and HPC Computer Science](https://doi.org/10.5281/zenodo.15306610)*

*See [README.md](README.md) for how to download or contribute to this checklist.*

## WHAT to include for a complete reproducible artifact

### Hardware
- [ ] Are detailed hardware resource requirements quantified and documented accurately (memory, disk space, network bandwidth, CPU specs, GPU specs, etc.)?
- [ ] Are clear instructions provided on how to access the required hardware (e.g., testbeds, cloud, proprietary access)?
- [ ] Is the minimum viable scale for reproduction of large-scale experiments specified?
- [ ] Are any specific hardware configurations (BIOS settings, power modes) that affect results documented?
- [ ] If specialized hardware is required, is there guidance for identifying functional equivalents or fallback configurations?

### Software
- [ ] Is all necessary source code with implementation details included?
- [ ] Are all software dependencies documented with specific version numbers or, if possible, specific repository commit hashes (which are static)?
- [ ] Has compatibility between licenses of all dependencies been verified and documented?
- [ ] Are configuration files with parameters used in the experiment provided?
- [ ] Are operating system requirements and tested versions specified?
- [ ] Is the execution environment (container, VM image) packaged when possible and appropriate (e.g., when the build process is not itself an integral part of the "reproducibility" or stopping condition for your experiment)?
- [ ] Is the process for obtaining necessary licenses for proprietary software documented?
- [ ] Is the exact version of the artifact used in the paper explicitly documented (e.g., Git commit hash, release version, DOI)?
- [ ] Are security considerations and assumptions documented, particularly for artifacts requiring privileged access?

### Data
- [ ] Are all necessary input datasets or generators included?
- [ ] For probabilistic experiments, are multiple input seeds or trial configurations provided to verify statistical significance?
- [ ] Are data versions, sources, and access methods specified?
- [ ] Are download scripts and persistent identifiers for large datasets provided to ensure data availability?
- [ ] Are sample or reduced datasets included for quick testing?
- [ ] Are any data preprocessing steps required documented?
- [ ] Are tools or scripts provided to validate input data integrity before experiments begin?

### Artifact Longevity
- [ ] Is the expected maintenance period for the artifact (a "best by" date) specified?
- [ ] Are persistent identifiers and repositories used for long-term access?
- [ ] Are dependencies that may affect longevity documented?
- [ ] Is contact information for future questions included?
