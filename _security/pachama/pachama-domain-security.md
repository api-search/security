---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pachama.com
  spf: true
hosts:
- cert_expires: Aug 21 11:12:40 2026 GMT
  host: pachama.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pachama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pachama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pachama
provider_slug: pachama
slug: pachama-domain-security
source_filename: pachama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pachama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:12:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pachama.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pachama/refs/heads/main/security/pachama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Carbon Credits
- Carbon Removal
- Carbon Markets
- Nature Based Solutions
- Forest Carbon
- Reforestation
- Afforestation
- REDD Plus
- MRV
- Monitoring Reporting Verification
- Satellite Imagery
- Remote Sensing
- Machine Learning
- Biomass Estimation
- Climate Tech
- Sustainability
- ESG
- Voluntary Carbon Market
---
