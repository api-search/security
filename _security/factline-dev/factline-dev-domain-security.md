---
api_specs:
- filename: factline-dev-free-api-openapi.yml
  format: yaml
  label: factline-dev Free API
  slug: factline-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factline-dev/openapi/factline-dev-free-api-openapi.yml
- filename: factline-dev-paid-x402-api-openapi.yml
  format: yaml
  label: factline-dev Paid (x402) API
  slug: factline-dev-paid-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factline-dev/openapi/factline-dev-paid-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: factline.dev
  spf: true
hosts:
- cert_expires: Jan  3 01:28:34 2027 GMT
  host: factline.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Factline Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for factline-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: factline-dev
provider_slug: factline-dev
slug: factline-dev-domain-security
source_filename: factline-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factline.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 01:28:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: factline.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/factline-dev/security/factline-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Compliance
- KYB
- API
---
