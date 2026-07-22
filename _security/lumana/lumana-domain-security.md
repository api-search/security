---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lumana.ai
  spf: true
hosts:
- cert_expires: Sep 22 15:11:37 2026 GMT
  host: lumana.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lumana
provider_slug: lumana
slug: lumana-domain-security
source_filename: lumana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:11:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lumana.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumana/refs/heads/main/security/lumana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Video Security
- AI
- Computer Vision
- Physical Security
- Surveillance
- Video Management
- Access Control
---
