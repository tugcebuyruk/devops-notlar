---
tags: [course, kodekloud]
course: DevOps Pre-Requisite Course
status: in progress
started: 2026-11-01
---
# DevOps Pre-Requisite Course

**Course link:** [KodeKloud — DevOps Pre-Requisite Course](https://learn.kodekloud.com/learn/courses/devops-pre-requisite-course)
**Related topics:** [[Linux]] · [[Networking Basics]] · [[Git]] · [[YAML]]

> Intro course covering the basics you need before DevOps tools (Docker, Kubernetes, Ansible...).
> Fix the section names to match the course order — add your notes under each section as you watch.

## Sections
### Introduction — the DevOps tools story
The big picture: how code travels from a developer's laptop to users, and which tool solves which problem.

```
development → Git repo → CI/CD pipeline → build → test → production
 (laptops)    (GitHub)   (Jenkins etc.)   (Docker image)   (Kubernetes)
```

| Problem | Solution | Tool |
|---|---|---|
| Many developers changing the same code | Store code in one shared place with history | [[Git]] / GitHub |
| Building, testing, deploying by hand is slow and error-prone | Automate every step in a pipeline | [[CI-CD]] (Jenkins, GitHub Actions) |
| "It works on my machine" — different setups on each server | Package the app with everything it needs | [[Docker]] (container image) |
| Too many containers to manage by hand; containers crash | Something decides where containers run and keeps them running | [[Kubernetes]] (container orchestration) |
| Human errors when setting up servers by hand → servers end up different | Define servers in code and create them automatically | [[Terraform]] / [[Ansible]] (Infrastructure as Code) |

**Container orchestration (Kubernetes):**
- It decides **which server** each container runs on.
- If a container fails (red one), it notices and **starts a new one** automatically → *self-healing*.
- If traffic grows, it adds more containers → *scaling*.

> 🇹🇷 Kubernetes bir orkestra şefi gibi: hangi container'ın hangi sunucuda çalışacağına karar verir, biri çökerse yerine yenisini başlatır.

### Linux basics → [[Linux]]
- 

### Vi editor
- 

### Package management (yum / apt)
- 

### Services (systemctl)
- 

### Networking basics (switching, routing, DNS) → [[Networking Basics]]
- 

### Application basics (Java, Node.js, Python, IPs and ports)
- 

### Git → [[Git]]
- 

### YAML / JSON → [[YAML]]
- 

## Questions / things I didn't get
- [ ] 

## Commands I learned
```bash

```
All commands: [[Linux Commands]] · [[Git Commands]]

Back: [[KodeKloud Courses]]
