# Solana Config Advisor & RPC Doctor (Hosted)

A hosted ReactJS web application on a custom domain that helps Solana validator operators and developers:

- **Config Advisor**: Generate a tuned validator configuration based on your intended hardware, with clear explanations for each setting.  
- **RPC Doctor**: Run quick, controlled performance tests on user-supplied RPC endpoints and view clear, exportable reports.

---

## Problem Statement
Validator configuration tuning is often guesswork, leading to wasted resources and reduced performance. RPC endpoints vary widely in reliability, but existing tools are either server-heavy or difficult to use. This project provides an accessible, hosted solution with clear recommendations and light-touch benchmarking.

---

## Features
- Input your hardware profile and receive an optimised validator config file.
- Explanations for all major configuration choices.
- Test RPC endpoints directly from the site (p50/p95 latency, success rate, errors).
- Export results in JSON or PDF.
- Save and compare hardware profiles and endpoint reports.

---

## Technology
- **Frontend**: ReactJS (single-page application)
- **Backend**: Node.js for config generation, RPC test orchestration, and security controls
- **Hosting**: Low-cost cloud host (~£25/month excluding domain)

---

## Security & Scalability
- Input validation and rate limiting
- No handling of private keys
- SSRF protection for outbound requests
- Easily scalable to meet demand

---

## Roadmap
**MVP**
- Config Advisor rules engine
- RPC Doctor bounded tests
- Result export (JSON/PDF)
- Save/load profiles and reports

**Future**
- Side-by-side comparisons
- Shareable public report links
- Optional user accounts
- Regional test runners

---

## Evaluation
- Unit tests for config generation
- Reliability and performance checks
- Usability testing with typical validator setups


