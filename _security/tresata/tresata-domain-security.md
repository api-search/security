---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tresata.ai
  spf: true
hosts:
- cert_expires: Oct 30 15:34:31 2026 GMT
  host: tresata.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tresata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tresata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tresata
provider_slug: tresata
slug: tresata-domain-security
source_filename: tresata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tresata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 15:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tresata.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tresata/refs/heads/main/security/tresata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Analytics
- Artificial Intelligence
- Machine-Learning
- Data Management
- Entity Resolution
- Big Data
- Enterprise Software
- Agents
---
