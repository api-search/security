---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: luminal.com
  spf: true
hosts:
- cert_expires: Sep 29 03:16:39 2026 GMT
  host: luminal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luminal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luminal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Luminal
provider_slug: luminal
slug: luminal-domain-security
source_filename: luminal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of luminal.com\nhosts:\n- host: luminal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: luminal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminal/refs/heads/main/security/luminal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- Compilers
- GPU
- Deep Learning
- Rust
- Developer Tools
- Open Source
---
