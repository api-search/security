---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: green-fusion.de
  spf: true
hosts:
- cert_expires: Oct 15 20:02:01 2026 GMT
  host: green-fusion.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Fusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Fusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Green Fusion
provider_slug: green-fusion
slug: green-fusion-domain-security
source_filename: green-fusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: green-fusion.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 20:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: green-fusion.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-fusion/refs/heads/main/security/green-fusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Energy
- Energy Management
- Heating
- Building Automation
- Sustainability
- Germany
- IoT
---
