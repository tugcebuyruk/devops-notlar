---
tags: [konu, yaml]
---
# YAML

## Nedir?
Girintiye dayalı, insan tarafından okunabilir yapılandırma formatı.

## Örnek
```yaml
uygulama:
  isim: web
  port: 8080
  ortamlar:
    - test
    - prod
```

## Dikkat
- Girinti **boşluk** ile yapılır, TAB kullanılmaz.
- `key: value` — iki noktadan sonra boşluk şart.

## Kullanıldığı yerler
- [[Kubernetes]] manifestleri · [[Ansible]] playbook'ları · [[CI-CD]] pipeline dosyaları · Docker Compose ([[Docker]])

Geri: [[00-Ana-Sayfa]]
