# MycoFabric: Bio-Inspired Unified Analytics for Microsoft Fabric

## Overview

This repository contains all code, synthetic data generators, experimental results, and publication figures from the MycoFabric paper submitted to the IEEE International Conference on Data Engineering 2025.

MycoFabric is a mycelium-inspired unified data processing framework that maps six core biological behaviors—hyphal growth, anastomosis, gradient-driven routing, compartmentalisation, symbiosis, and sporulation—onto Microsoft Microsoft Fabric component architecture.

---

## Experiments

This repository includes 5 complete experiments that validate the MycoFabric framework:

| Experiment | Description                                                         | Status   |
| ---------- | ------------------------------------------------------------------- | -------- |
| E1         | Ingestion Throughput — Measures how fast data can be ingested       | Complete |
| E2         | Anastomosis Overhead — Quantifies stream-batch MERGE operation cost | Complete |
| E3         | Gradient Routing — Tests workload classifier accuracy               | Complete |
| E4         | Fault Recovery — Measures compartmentalised self-healing            | Complete |
| E5         | Storage Efficiency — Compares storage footprint vs Lambda/Kappa     | Complete |

---

## Key Results

| Metric                    | MycoFabric Result                                     |
| ------------------------- | ----------------------------------------------------- |
| Max Throughput            | 44,000 events/sec (88% efficiency at 50K/s target)    |
| Anastomosis Overhead      | 2.9 - 6.7 seconds (depending on duplicate rate)       |
| Gradient Routing Accuracy | 85% (boundary cases) / 100% (clean separation, n=100) |
| Fault Recovery (MTTR)     | 2 seconds (60× faster than manual restart)            |
| Data Loss on Failure      | 0 events (vs 100 events lost in baseline)             |
| Storage (1 workspace)     | 1,000 GB                                              |
| Storage (3 workspaces)    | 1,000 GB (67% savings vs Lambda)                      |

---

## Repository Structure
