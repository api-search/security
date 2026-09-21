---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airloom.energy
  spf: true
hosts:
- cert_expires: Nov 21 03:21:06 2026 GMT
  host: www.airloom.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airloom Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airloom Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airloom Energy
provider_slug: airloom-energy
slug: airloom-energy-domain-security
source_filename: airloom-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airloom.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 03:21:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: airloom.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airloom-energy/refs/heads/main/security/airloom-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Wind Energy
- Renewable Energy
- Clean Energy
- Hardware
- Climate Tech
- Utilities
---
