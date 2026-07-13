---
api_specs:
- filename: green-screens-ai-openapi.yml
  format: yaml
  label: Green Screens AI Prediction API
  slug: prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greenscreens.ai
  spf: true
hosts:
- host: www.greenscreens.ai
  https: false
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: connect.greenscreens.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Screens Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Screens AI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Green Screens AI
provider_slug: green-screens-ai
slug: green-screens-ai-domain-security
source_filename: green-screens-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greenscreens.ai\n  https: false\n- host: connect.greenscreens.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: greenscreens.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/security/green-screens-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Freight
- Logistics
- Machine Learning
- Pricing
- Transportation
---
