---
tags: [topic, certification]
updated: 2026-11-09
---
# Certifications

> The Kubernetes and Red Hat Ansible certification exams are all done on Linux systems — another reason to learn [[Linux]] well.
> Prices and rules change — always check the official page before booking.

## Kubernetes (CNCF / Linux Foundation) → [[Kubernetes]]
| Exam | Level | Format | Notes |
|---|---|---|---|
| **KCNA** | Beginner | Multiple choice, 90 min | Good first step, no terminal |
| **CKAD** | Developer | Hands-on, 2 h | Deploy and run apps on Kubernetes |
| **CKA** | Administrator | Hands-on, 2 h | Most popular — build and fix clusters |
| **CKS** | Security | Hands-on, 2 h | Requires an active CKA |

**Hands-on exams (CKA / CKAD / CKS):**
- No multiple choice — you solve 15–20 real tasks in a **Linux terminal** with `kubectl`.
- Passing score: 66% (CKS 67%). One free retake included.
- Official docs (kubernetes.io) allowed during the exam.
- Remote, online, with webcam (proctored).
- Price: around $445 (list) — Linux Foundation often has discounts (e.g. Cyber Monday).
- Includes 2 sessions of the **killer.sh** practice exam simulator.

## Red Hat Ansible → [[Ansible]]
| Exam | What | Format |
|---|---|---|
| **EX200 – RHCSA** | Linux system administration (prerequisite) | Hands-on |
| **EX294 – RHCE** | Ansible automation on RHEL 9 | Hands-on, 4 h |

**EX294:**
- Write Ansible **playbooks** to automate real RHEL (Red Hat Enterprise Linux) systems.
- You work on a **control node** + several **managed nodes** (all Linux).
- Passing score: 210/300 (70%). Only Red Hat's own docs allowed.
- Price: around $450–500 (varies by country).
- Red Hat now also calls this credential *"Red Hat Certified Advanced System Administrator in Ansible"*.

## My path (suggested)
1. Finish Linux basics → (optional) KCNA
2. Docker → Kubernetes → **CKAD** or **CKA**
3. Ansible → RHCSA → RHCE (later)

KodeKloud has prep courses + mock exams for all of these.

Back: [[00-Home]]
