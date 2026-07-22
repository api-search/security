---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: verisimlife.com
  spf: true
hosts:
- cert_expires: Oct  3 03:00:29 2026 GMT
  host: verisimlife.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verisim Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VeriSIM Life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VeriSIM Life
provider_slug: verisim-life
slug: verisim-life-domain-security
source_filename: verisim-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verisimlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verisimlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisim-life/refs/heads/main/security/verisim-life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Biology
- Drug Discovery
- Artificial Intelligence
- Life Sciences
- Pharmaceutical
- Biosimulation
- Machine Learning
---
