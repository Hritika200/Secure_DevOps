# Secure DevOps — Cloud Infrastructure & Observability

A personal project to practice end-to-end secure cloud deployment:
provisioning infrastructure as code, containerising a full-stack application,
and building a real-time log observability stack.

## Stack

- **Frontend** — React
- **Backend** — Flask
- **Containerisation** — Docker + Docker Compose
- **Infrastructure** — GCP VM, provisioned with Terraform
- **Observability** — ELK Stack + Fluent Bit for log ingestion, New Relic APM

## What it does

- Provisions a GCP VM end-to-end using Terraform (IaC)
- Deploys containerised frontend and backend services via Docker Compose
- Captures and indexes STDOUT logs from both services using Fluent Bit → Elasticsearch
- Makes logs queryable through a Kibana dashboard
- Monitors backend application performance with New Relic APM

## Key learnings

- Infrastructure as Code principles: resource definition, validation, automated deployment
- Log ingestion pipeline design: getting structured logs from containers into a searchable index
- Connecting APM tooling to a live service for real observability
