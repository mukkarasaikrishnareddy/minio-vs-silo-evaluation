# MinIO vs Silo Evaluation

## Project Overview

This project evaluates Silo, a community-maintained MinIO fork, as a potential replacement for the last open-source MinIO Community Edition release.

The evaluation uses a local Docker Compose laboratory to compare functionality, compatibility, data integrity, cluster behavior, performance, security, and maintenance considerations.

## Objectives

- Verify S3 API and client compatibility.
- Evaluate object versioning, object lock, and lifecycle policies.
- Test cluster health, healing, and replication behavior.
- Compare performance using Warp under equivalent resource constraints.
- Validate object integrity using manifests, checksums, and client tools.
- Assess compatibility conditions O01–O08.
- Document security risks, licensing, maintenance, and limitations.

## Environment

- Host OS: Windows 11
- Container runtime: Docker Desktop with the WSL 2 backend
- Orchestration: Docker Compose v2
- Shared Docker network: `migration-net`
- Test data: Synthetic data only
- Infrastructure: Local workstation; no cloud resources

Exact software versions, image digests, configuration, and resource limits will be recorded in the environment documentation.

## Repository Structure

- `compose/` — Docker Compose configurations
- `scripts/` — Reusable test and verification scripts
- `tests/` — Functional and compatibility tests
- `benchmarks/` — Performance test configurations and results
- `docs/` — Sub-task procedures and evidence
- `reports/` — Final comparison and recommendation

## Evidence Policy

Every test records its procedure, expected result, actual result, and PASS/FAIL status. Raw command output is retained alongside relevant screenshots.

No real customer data or unredacted credentials are used.

## Project Status

Phase 1: Environment preparation and repository setup.

No compatibility or performance conclusions have been established yet.