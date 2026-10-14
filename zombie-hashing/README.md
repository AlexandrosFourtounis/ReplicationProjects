# Zombie Hashing Replication

**Collaborative project:** Alexandros Fourtounis and Anna Makridou, University of Crete.  
**Course:** CS543.

**Original paper:** [Zombie Hashing: Reanimating Tombstones in a Graveyard](https://doi.org/10.1145/3725424), Yuvaraj Chesetti et al., SIGMOD 2025.  
**Authors' implementation:** [saltsystemslab/ZombieHT](https://github.com/saltsystemslab/ZombieHT).

## Study

Replicated throughput, home-slot distance, and operation-latency experiments (Figures 6a, 9a/c, 10a, and Table 5) on an AWS EC2 `t2.large` instance with 2 vCPUs and 8 GB RAM.

- Reduced table capacity from 2^27 to 2^24 slots and excluded the unsupported IcebergHT baseline.
- Patched a compiler incompatibility and developed headless Python plotting scripts for partial benchmark runs.
- Compared compact and vectorized Zombie Hashing against competing hash tables under churn workloads.

**Findings:** The reproduced trends supported stable Zombie Hashing throughput and lower maximum insertion latency than GraveyardHT. Smaller tables and different hardware affected absolute performance.

**Materials:** [Report](zombie-hashing-replication-report.pdf)

[Back to all projects](../README.md)
