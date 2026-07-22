---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hycu.com
  spf: true
hosts:
- cert_expires: Oct 15 11:28:02 2026 GMT
  host: www.hycu.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hycu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HYCU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HYCU
provider_slug: hycu
slug: hycu-domain-security
source_filename: hycu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hycu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:28:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: hycu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hycu/refs/heads/main/security/hycu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Infrastructure
- Data Protection
- Backup
- Disaster Recovery
- Ransomware
- Data Resilience
- SaaS
- Cloud
---
