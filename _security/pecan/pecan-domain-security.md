---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pecan.ai
  spf: true
hosts:
- cert_expires: Sep 16 07:31:40 2026 GMT
  host: www.pecan.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pecan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pecan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pecan
provider_slug: pecan
slug: pecan-domain-security
source_filename: pecan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pecan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pecan.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pecan/refs/heads/main/security/pecan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Predictive Analytics
- Machine Learning
- Data Science
- Forecasting
- Business Intelligence
---
