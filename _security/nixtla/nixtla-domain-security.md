---
api_specs:
- filename: nixtla-openapi-original.json
  format: json
  label: Nixtla Forecast API
  slug: nixtla-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-openapi-original.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:eduardo@nixtla.io"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nixtla.io
  spf: true
hosts:
- cert_expires: Oct  3 19:51:24 2026 GMT
  host: nixtla.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:32:42 2026 GMT
  host: api.nixtla.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nixtla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nixtla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nixtla
provider_slug: nixtla
slug: nixtla-domain-security
source_filename: nixtla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nixtla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nixtla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:32:42 2026 GMT\n  hsts: null\ndomains:\n- domain: nixtla.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:eduardo@nixtla.io\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/security/nixtla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Time Series
- Forecasting
- Anomaly Detection
- Machine Learning
- Artificial Intelligence
- Foundation Model
- Predictive Analytics
- Data Science
---
