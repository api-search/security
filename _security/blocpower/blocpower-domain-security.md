---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blocpower.io
  spf: true
hosts:
- cert_expires: Aug 24 22:24:56 2026 GMT
  host: www.blocpower.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blocpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlocPower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BlocPower
provider_slug: blocpower
slug: blocpower-domain-security
source_filename: blocpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blocpower.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:24:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blocpower.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blocpower/refs/heads/main/security/blocpower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- Building Decarbonization
- Energy Efficiency
- Electrification
- Clean Energy
- Sustainability
- Public Benefit Corporation
---
