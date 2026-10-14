# TUNA Replication

**Individual project:** Alexandros Fourtounis, University of Crete.  
**Course:** CS559.

**Original paper:** [TUNA: Tuning Unstable and Noisy Cloud Applications](https://arxiv.org/abs/2503.01801), Johannes Freischuetz et al., EuroSys 2025.  
**Authors' implementation:** [uw-mad-dash/TUNA](https://github.com/uw-mad-dash/TUNA).

## Study

Evaluated noise sensitivity and tuning efficiency using PostgreSQL 16.1 with TPC-C and Epinions workloads on Azure, with one orchestrator and two workers.

- Adapted workloads and container memory limits for 2-vCPU, 8-GB nodes.
- Resolved deployment, Docker networking, Ray code synchronization, and pandas compatibility issues.
- Processed experiment outputs and compared latency convergence with a random-search baseline.

**Findings:** Noise-free runs converged earlier. TUNA reduced latency from approximately 190 ms to 160 ms over the first 12 trials. Memory exhaustion limited the initial comparison and required further workload reduction.

**Materials:** [Report](tuna-replication-report.pdf) | [Presentation](tuna-replication-presentation.pdf)

[Back to all projects](../README.md)
