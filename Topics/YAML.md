---
tags: [topic, yaml]
---
# YAML

## What is it?
A human-readable, indentation-based configuration format.

## Example
```yaml
app:
  name: web
  port: 8080
  environments:
    - test
    - prod
```

## Watch out
- Indent with **spaces**, never TAB.
- `key: value` — a space after the colon is required.

## Where it's used
- [[Kubernetes]] manifests · [[Ansible]] playbooks · [[CI-CD]] pipeline files · Docker Compose ([[Docker]])

Back: [[00-Home]]
