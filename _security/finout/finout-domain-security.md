---
api_specs:
- filename: finout-api-openapi.yml
  format: yaml
  label: Finout
  slug: finout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/openapi/finout-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finout.io
  spf: true
hosts:
- cert_expires: Sep 22 05:45:27 2026 GMT
  host: www.finout.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: app.finout.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finout, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finout
provider_slug: finout
slug: finout-domain-security
source_filename: finout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finout.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:45:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.finout.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finout.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/security/finout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Budgets
- Costs
- FinOps
---
