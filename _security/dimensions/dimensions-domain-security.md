---
api_specs:
- filename: dimensions-openapi.yml
  format: yaml
  label: Dimensions Analytics API
  slug: dimensions-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/openapi/dimensions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dimensions.ai
  spf: true
hosts:
- cert_expires: Sep  2 09:06:02 2026 GMT
  host: www.dimensions.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: docs.dimensions.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: app.dimensions.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dimensions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dimensions, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dimensions
provider_slug: dimensions
slug: dimensions-domain-security
source_filename: dimensions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dimensions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:06:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.dimensions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\n- host: app.dimensions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dimensions.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/security/dimensions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Research
- Publications
- Grants
- Patents
- Clinical Trials
- Jupyter Notebooks
---
