# Solana Validator Performance Autotuner

## Problem Statement
Running a Solana validator is resource-intensive and expensive, requiring high-end hardware such as fast NVMe solid-state drives, large amounts of RAM, and powerful central processing units.  
Despite this, most validator operators rely on guesswork when tuning performance-related configurations, such as:

- Account index memory limits
- Snapshot intervals
- Ledger compaction schedules
- Thread and leader scheduling parameters
- Disk and RAM trade-offs

Poor configuration choices can lead to missed slots, increased skipped rates, wasted resources, and ultimately reduced rewards.  
At present, there is no ready-to-use system that automates the process of tuning and optimising validator performance.

---

## Project Goal
To design and implement a self-optimising system that:
1. Deploys a Solana validator node to the testnet using Infrastructure-as-Code.
2. Automates configuration testing by varying performance-related parameters.
3. Monitors and collects both blockchain-level and system-level performance metrics.
4. Analyses results to determine the most efficient configuration for a given hardware profile.
5. Produces recommendations and a downloadable, ready-to-use configuration file.

---

## Planned Implementation

### For the User:
- Deploy a Solana validator on the testnet with preconfigured Infrastructure-as-Code scripts.
- Start the autotuning process — the system will:
  - Apply a range of tested configuration profiles.
  - Monitor real-time performance through an integrated dashboard.
  - Record results for later analysis.
- View results on a metrics dashboard showing:
  - Vote credits
  - Skipped slots
  - Block production success rate
  - CPU and RAM usage
  - Disk input/output operations
  - Network throughput
- Receive an optimisation report that includes:
  - The best configuration for their hardware
  - Expected performance gains
  - Any cost-saving recommendations

---

## Key Features
- Automated deployment using Infrastructure-as-Code for repeatable setups.
- Integrated observability to monitor performance metrics.
- Automated benchmarking engine to test different configurations.
- Data-driven recommendations for validator operators.

---

## Outcome
The Validator Performance Autotuner will enable Solana node operators to:
- Maximise rewards by optimising block production and voting performance.
- Reduce infrastructure costs while maintaining performance.
- Gain deeper insight into how configuration choices affect validator efficiency.
