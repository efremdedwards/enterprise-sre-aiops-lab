# Current Kubernetes Workload

## Purpose

This document captures the existing Kubernetes application workload used as the first application stack for the Enterprise SRE / AIOps lab.

## Current Stack

| Component | Name | Type | Status |
|---|---|---|---|
| Web app pod | `webapp-deployment-68f5c4445b-d4lq4` | Pod | Running |
| MongoDB pod | `mongo-deployment-6f869b8d8b-4wlxn` | Pod | Running |
| Web app service | `webapp-service` | NodePort | Running |
| MongoDB service | `mongo-service` | ClusterIP | Running |
| Web app deployment | `webapp-deployment` | Deployment | Available |
| MongoDB deployment | `mongo-deployment` | Deployment | Available |

## Service Details

| Service | Type | Cluster IP | Port Mapping |
|---|---|---|---|
| `webapp-service` | NodePort | `10.100.82.248` | `3000:30100/TCP` |
| `mongo-service` | ClusterIP | `10.106.19.194` | `27017/TCP` |
| `kubernetes` | ClusterIP | `10.96.0.1` | `443/TCP` |

## Deployment Details

| Deployment | Ready | Up-to-date | Available | Age |
|---|---:|---:|---:|---|
| `mongo-deployment` | 1/1 | 1 | 1 | 3d4h |
| `webapp-deployment` | 1/1 | 1 | 1 | 3d4h |

## Architecture

```text
Client / Browser / curl
   ↓
Node IP:30100
   ↓
webapp-service
   ↓
webapp-deployment pod
   ↓
mongo-service
   ↓
mongo-deployment pod
