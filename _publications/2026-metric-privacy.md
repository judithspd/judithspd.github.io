---
title: "Metric-privacy-inspired noise calibration in federated learning: Improving convergence and preventing client inference attacks"
collection: publications
permalink: /publication/2026-metric-privacy
date: 2026-04-16
venue: 'Knowledge-Based Systems'
paperurl: 'https://doi.org/10.1016/j.knosys.2026.115993'
citation: 'Sáinz-Pardo Díaz, J., Athanasiou, A., Jung, K., Palamidessi, C., & López García, Á. (2026). Metric-privacy-inspired noise calibration in federated learning: Improving convergence and preventing client inference attacks. Knowledge-Based Systems, 115993. DOI: https://doi.org/10.1016/j.knosys.2026.115993'
---

**Abstract**
Federated learning (FL) enables the training of a global model across multiple data owners (clients) without sharing raw data. This distributed architecture is orchestrated by a central server that aggregates the local models from the clients. In cases where the server is trusted but not all network nodes, differential privacy (DP) can be used to privatize the aggregated model by adding noise. However, this may affect convergence across the FL rounds. In this work, we build on the notion of metric-privacy as a design principle to calibrate the noise added by the server under a global-DP setting, with the objective of mitigating its impact on the convergence of the aggregated model. We do not enforce metric-privacy as a formal guarantee, but rather use it to guide noise calibration. We compare our approach with vanilla FL and global-DP by analyzing the impact on six aggregation strategies and applying it to a medical imaging use case, simulating different scenarios with homogeneous and non-i.i.d. clients. Finally, we introduce the client inference attack (CIA), where a semi-honest client tries to find whether another client participated in the training and study how it can be mitigated using DP and metric-aware noise calibration. Our experiments show that metric-privacy aware noise calibration strategy improves the accuracy compared to standard DP in all the scenarios analyzed, while achieving a comparable success rate against CIA. These results indicate that metric-privacy inspired noise calibration can deliver a superior utility-privacy trade-off in medical-imaging federated settings.

