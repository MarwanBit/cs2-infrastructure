"""CS2 Match Predictor - Infrastructure Orchestration

This repository orchestrates deployment of all microservices from separate repositories.
Uses Terraform to provision infrastructure and deploy services.

## Structure Overview

- `terraform/` - Infrastructure provisioning (local & production)
- `scripts/` - Deployment and orchestration scripts
- `services/` - Cloned service repositories (git submodules or manual clone)
- `e2e/` - End-to-end tests
- `docker-compose.yml` - Local development orchestration
"""
