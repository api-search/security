---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deeploi.io
  spf: true
hosts:
- cert_expires: Aug 31 17:18:28 2026 GMT
  host: www.deeploi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deeploi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deeploi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deeploi
provider_slug: deeploi
slug: deeploi-domain-security
source_filename: deeploi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deeploi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deeploi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deeploi/refs/heads/main/security/deeploi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- IT Management
- ITSM
- Device Management
- Employee Onboarding
- Cybersecurity
- Compliance
- DACH
- MDM
---
