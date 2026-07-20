---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coiled.io
  spf: true
hosts:
- cert_expires: Sep 10 12:40:22 2026 GMT
  host: coiled.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coiled Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coiled, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coiled
provider_slug: coiled
slug: coiled-domain-security
source_filename: coiled-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coiled.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:40:22 2026 GMT\n  hsts: false\ndomains:\n- domain: coiled.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coiled/refs/heads/main/security/coiled-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Cloud Computing
- Data Science
- Dask
- Python
- Distributed Computing
- Machine Learning
- Serverless
---
