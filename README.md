# Enterprise SRE / AIOps Lab

## Purpose

This repository is a personal enterprise-style Site Reliability Engineering lab. The goal is to practice building, operating, monitoring, troubleshooting, and automating a Kubernetes-based application environment using tools and workflows commonly found in production cloud operations.

This lab is also intended to support hands-on practice for SRE, cloud operations, DevOps, Kubernetes, observability, incident response, and AI-assisted operations.

## Current Environment

| Component | Tool / Platform | Status |
|---|---|---|
| Virtualization | VirtualBox | Running |
| Operating System | Ubuntu Server | Running |
| Kubernetes | 1 control-plane node and 1 worker node | Running |
| Containers | Docker | Running |
| Source Control | GitHub | In Progress |
| Project Tracking | Jira | In Progress |
| Documentation | Confluence / Markdown | In Progress |
| AI Coding Assistant | GitHub Copilot | Installed |

## Planned Stack

| Area | Tool / Approach |
|---|---|
| Version Control | Git + GitHub |
| Pull Requests | GitHub Pull Requests |
| CI | GitHub Actions |
| CD / GitOps | Argo CD |
| Infrastructure as Code | Terraform |
| Application | Python Flask API |
| Database | PostgreSQL |
| Monitoring | Prometheus + Grafana |
| Logging | Loki + Promtail |
| Data Pipeline | Python ETL script |
| Incident Response | Simulated production failures + RCA notes |
| AI/SRE Assistant | Python-based AI incident triage workflow |

## Lab Goals

1. Build and operate a Kubernetes-based application platform.
2. Use GitHub branches and pull requests for change control.
3. Automate validation with GitHub Actions.
4. Deploy workloads to Kubernetes using manifests and later GitOps.
5. Manage infrastructure and application configuration with Terraform.
6. Add observability using Prometheus and Grafana.
7. Add centralized logging using Loki and Promtail.
8. Simulate production incidents and document root-cause analysis.
9. Build an AI-assisted incident triage workflow for logs, alerts, and Kubernetes events.

## Project Workflow

Work is tracked in Jira using a Kanban-style workflow:

```text
To Do → In Progress → Blocked → PR Open → Testing → Done
