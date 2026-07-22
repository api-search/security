---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polaron.ai
  spf: true
hosts:
- cert_expires: Aug 21 18:13:05 2026 GMT
  host: polaron.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polaron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polaron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Polaron
provider_slug: polaron
slug: polaron-domain-security
source_filename: polaron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polaron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:13:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polaron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polaron/refs/heads/main/security/polaron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Materials Science
- Artificial Intelligence
- Machine Learning
- Microscopy
- Microstructure
- Batteries
- Additive Manufacturing
- Deep Tech
- Simulation
---
