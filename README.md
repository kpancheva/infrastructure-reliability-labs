# Infrastructure Reliability Labs

### Linux | Kubernetes | DNS | Incident Response

A hands-on infrastructure engineering project focused on deploying, troubleshooting, and recovering Linux and Kubernetes services.

## About This Project

I created this repository as part of a **5-day technical challenge** to strengthen and demonstrate my practical knowledge of Linux administration, Kubernetes networking, DNS infrastructure, and incident response.

Rather than simply memorizing commands or studying theoretical concepts, my goal is to build functional infrastructure, deliberately introduce failures, investigate their root causes, and restore services.

Each lab follows the same engineering workflow:

**Build → Validate → Break → Investigate → Recover → Document**

## Lab Progress

| Day | Focus 
|---|---
| Day 01 | Kubernetes DNS & PowerDNS Incident Recovery 
| Day 02 | Linux Service Administration & Troubleshooting 
| Day 03 | Kubernetes Operations & Troubleshooting 
| Day 04 | Advanced DNS & Network Diagnostics 
| Day 05 | Infrastructure Incident Response 

## Day 01 — Kubernetes DNS & PowerDNS

**Objective:** Deploy an authoritative DNS server inside Kubernetes, configure DNS records, verify resolution over UDP and TCP, and investigate a simulated networking failure.

**Technologies:** Kubernetes, PowerDNS, CoreDNS, Linux, YAML, `kubectl`, `dig`, `nslookup`.

**What I accomplished:**
- Inspected a two-node Kubernetes cluster and its DNS infrastructure.
- Deployed PowerDNS using a ConfigMap, Deployment, and ClusterIP Service.
- Configured the authoritative `demo.test` zone.
- Verified DNS resolution over UDP and TCP.
- Simulated a DNS outage by changing a Kubernetes Service selector.
- Diagnosed missing Service endpoints and restored DNS resolution.

**Key takeaway:** A running Pod does not guarantee that its Service is accessible. Effective troubleshooting requires understanding the relationship between Pods, labels, Services, and EndpointSlices.

Detailed configuration, troubleshooting commands, and evidence will be documented in `day-01-kubernetes-dns/`.

## Tools & Environment

- **Lab environment:** Killercoda browser-based playgrounds
- **Infrastructure:** Kubernetes and Linux
- **DNS:** CoreDNS and PowerDNS
- **Diagnostics:** kubectl, dig, nslookup, and Linux command-line tools
- **Version control and documentation:** GitHub, Git, Markdown

## Engineering Approach

These labs are self-directed simulations in isolated learning environments, not production incidents.

Each exercise documents the initial infrastructure state, the deliberately introduced failure, the diagnostic evidence, the root cause, the corrective action, and verification of recovery.

## Project Goal

Develop a practical, reproducible portfolio of infrastructure troubleshooting scenarios that demonstrates systematic problem-solving, technical documentation, and an understanding of Linux, Kubernetes, and DNS reliability.
