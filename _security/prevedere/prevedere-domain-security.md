---
api_specs:
- filename: prevedere-openapi-original.json
  format: json
  label: Board Foresight API (V1)
  slug: board-foresight-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prevedere.com
  spf: false
hosts:
- cert_expires: Sep 23 19:21:27 2026 GMT
  host: prevedere.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 13:26:45 2026 GMT
  host: api.prevedere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prevedere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prevedere, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Prevedere
provider_slug: prevedere
slug: prevedere-domain-security
source_filename: prevedere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prevedere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:21:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prevedere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 13:26:45 2026 GMT\n  hsts: null\ndomains:\n- domain: prevedere.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/security/prevedere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Economic Forecasting
- Predictive Analytics
- Demand Planning
- Financial Planning
- Macroeconomic Data
- Indicators
- Time Series
- Data Integration
- Machine Learning
---
