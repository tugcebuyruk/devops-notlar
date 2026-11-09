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

**Infrastructure as Code (IaC):**
- **Terraform** → *creates* the servers (provisioning).
- **Ansible** → *configures* the servers: installs software, sets them up. Instructions are written in a `playbook.yaml`.

Example from the video — an Ansible playbook that sets up a Kubernetes cluster:
```yaml
- name: apply common configuration to all nodes
  hosts: all              # which servers → all of them
  remote_user: root       # log in as root
  roles:
    - common              # what to do → the "common" setup

- name: configure and deploy the controlplane
  hosts: controlplane     # only the Kubernetes "manager" servers
  roles:
    - kubernetes controlplane

- name: configure and deploy workers
  hosts: workers          # only the servers that run containers
  roles:
    - kubernetes workers
```
Each block = **which servers** (`hosts`) + **what to do** (`roles`). Same file → every server set up the same way, no human errors.

**Monitoring:**
- **Prometheus** → collects metrics (CPU, memory, errors...) from all servers and stores them centrally.
- **Grafana** → turns those metrics into dashboards and graphs.
- → [[Monitoring]]

**The DevOps loop (∞):**
```
idea → Plan → Code → Build → Test → Release → Deploy → Operate → Monitor
                 ↑                                                │
                 └──────────────── Feedback ──────────────────────┘
```
It never ends: what we learn from monitoring and user feedback becomes the next idea.
All these tools together take us **from an idea to the user, fast and reliably**. → [[What is DevOps]]

### Linux basics → [[Linux]]
#### Why Linux?
- Most DevOps tools **require Linux** — so learning Linux basics comes first.
- Stack Overflow Developer Survey 2019:
  - Linux was the **most used** platform (53.3%), ahead of Windows (50.7%).
  - Linux was the **most loved** platform (83.1%), followed by Docker and Kubernetes.
- DevOps tools were born on Linux; Windows support came later or is limited:

| Tool | Linux vs Windows |
|---|---|
| [[Docker]] | Born on Linux in 2013; Docker for Windows came only in 2016 |
| [[Ansible]] | Can *manage* Windows servers, but cannot *run* on Windows (only inside WSL) |
| [[Kubernetes]] | The control plane (the "master" / manager part) runs only on Linux |

> **WSL** (Windows Subsystem for Linux) = a way to run Linux inside Windows.

**✍️ My notes (from my notebook):**
- For example, containerization tools like Docker were only available on Linux-based systems for many years.
- Even though Ansible can manage Windows systems as target machines, a Linux system is required to be the **Ansible controller**.
  - *controller* (control node) = the machine where Ansible is installed and run from · *target* (managed node) = the machines it configures

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
