---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: climavision.com
  spf: true
hosts:
- cert_expires: Aug 24 01:57:51 2026 GMT
  host: climavision.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climavision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climavision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Climavision
provider_slug: climavision
slug: climavision-domain-security
source_filename: climavision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: climavision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: climavision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climavision/refs/heads/main/security/climavision-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Weather Intelligence
- Forecasting
- Numerical Weather Prediction
- Weather Radar
- X-Band Radar
- Dual Polarization
- Gap-Filling Radar
- Radar as a Service
- AI Forecasting
- Horizon AI
- Renewable Energy
- Severe Weather
- Hurricane
- Aviation Weather
- Agriculture
- Energy
- Insurance
---
