---
api_specs:
- filename: cube-planning-openapi-original.yml
  format: yaml
  label: Cube API
  slug: cube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-planning/refs/heads/main/openapi/cube-planning-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cubesoftware.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.cubesoftware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cube Planning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cube Planning, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cube Planning
provider_slug: cube-planning
slug: cube-planning-domain-security
source_filename: cube-planning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.cubesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cubesoftware.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cube-planning/refs/heads/main/security/cube-planning-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- Analytics
- Planning
---
