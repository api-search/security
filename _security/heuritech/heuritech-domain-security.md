---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heuritech.com
  spf: true
hosts:
- cert_expires: Nov  9 23:43:49 2026 GMT
  host: heuritech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heuritech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heuritech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heuritech
provider_slug: heuritech
slug: heuritech-domain-security
source_filename: heuritech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heuritech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heuritech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/security/heuritech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Machine Learning
- Fashion
- Trend Forecasting
- Demand Forecasting
- Retail
- Luxury
- Market Intelligence
- Consumer Insights
- Social Media Analytics
---
