---
api_specs:
- filename: two-api-key-api-openapi.yml
  format: yaml
  label: Two API Key API
  slug: two-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-api-key-api-openapi.yml
- filename: two-invoice-api-openapi.yml
  format: yaml
  label: Two Invoice API
  slug: two-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-invoice-api-openapi.yml
- filename: two-order-api-openapi.yml
  format: yaml
  label: Two Order API
  slug: two-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-order-api-openapi.yml
- filename: two-order-intent-api-openapi.yml
  format: yaml
  label: Two Order intent API
  slug: two-order-intent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-order-intent-api-openapi.yml
- filename: two-settlement-report-api-openapi.yml
  format: yaml
  label: Two Settlement report API
  slug: two-settlement-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-settlement-report-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: two.inc
  spf: true
hosts:
- cert_expires: Jan 26 09:06:34 2027 GMT
  host: www.two.inc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Two Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Two, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Two
provider_slug: two
slug: two-domain-security
source_filename: two-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.two.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 09:06:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: two.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/two/security/two-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B Payments
- FinTech
- API Platform
- Checkout
- Trade Accounts
---
