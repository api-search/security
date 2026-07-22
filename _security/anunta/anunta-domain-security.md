---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anunta.com
  spf: true
hosts:
- cert_expires: Dec  5 12:09:23 2026 GMT
  host: www.anunta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anunta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anunta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Anunta
provider_slug: anunta
slug: anunta-domain-security
source_filename: anunta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anunta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 12:09:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anunta.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anunta/refs/heads/main/security/anunta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Desktop as a Service
- DaaS
- Virtual Desktop Infrastructure
- VDI
- Cloud Services
- Managed Endpoints
- Enterprise IT
---
