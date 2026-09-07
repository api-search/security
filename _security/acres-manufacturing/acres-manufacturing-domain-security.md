---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acresmanufacturing.com
  spf: true
hosts:
- cert_expires: Nov  3 19:26:17 2026 GMT
  host: acresmanufacturing.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acres Manufacturing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acres Manufacturing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acres Manufacturing
provider_slug: acres-manufacturing
slug: acres-manufacturing-domain-security
source_filename: acres-manufacturing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acresmanufacturing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: acresmanufacturing.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acres-manufacturing/refs/heads/main/security/acres-manufacturing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Casino Gaming
- Casino Management System
- Gaming Technology
- Slot Machines
- Cashless Payments
- Real-Time Data
- Event Streaming
- WebSocket
- Bluetooth Low Energy
- Loyalty and Bonusing
- Hospitality
---
