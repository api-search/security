---
api_specs:
- filename: cubesoftware-openapi-original.yml
  format: yaml
  label: Cube API
  slug: cube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubesoftware/refs/heads/main/openapi/cubesoftware-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cubesoftware.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: cubesoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.cubesoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cubesoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cube, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cube
provider_slug: cubesoftware
slug: cubesoftware-domain-security
source_filename: cubesoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cubesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cubesoftware.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubesoftware/refs/heads/main/security/cubesoftware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- Analytics
- Spreadsheets
- SaaS
---
