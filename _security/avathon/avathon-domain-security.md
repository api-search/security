---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avathon.com
  spf: true
hosts:
- cert_expires: Oct 17 04:27:16 2026 GMT
  host: avathon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avathon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avathon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avathon
provider_slug: avathon
slug: avathon-domain-security
source_filename: avathon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avathon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 04:27:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avathon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avathon/refs/heads/main/security/avathon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Industrial AI
- Predictive Maintenance
- Asset Performance Management
- Computer-Vision
- Digital Twin
- Renewable Energy
- Oil and Gas
- Manufacturing
- Aerospace and Defense
- Logistics
---
