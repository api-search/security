---
api_specs:
- filename: hunchsheet-app-ask-api-openapi.yml
  format: yaml
  label: Hunch Ask API
  slug: hunchsheet-app-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-ask-api-openapi.yml
- filename: hunchsheet-app-balance-api-openapi.yml
  format: yaml
  label: Hunch Balance API
  slug: hunchsheet-app-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-balance-api-openapi.yml
- filename: hunchsheet-app-checkout-api-openapi.yml
  format: yaml
  label: Hunch Checkout API
  slug: hunchsheet-app-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-checkout-api-openapi.yml
- filename: hunchsheet-app-quote-api-openapi.yml
  format: yaml
  label: Hunch Quote API
  slug: hunchsheet-app-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-quote-api-openapi.yml
- filename: hunchsheet-app-trial-api-openapi.yml
  format: yaml
  label: Hunch Trial API
  slug: hunchsheet-app-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-trial-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: hunchsheet.app
  spf: false
hosts:
- cert_expires: Jan 23 21:20:27 2027 GMT
  host: hunchsheet.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hunch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hunch
provider_slug: hunchsheet-app
slug: hunchsheet-app-domain-security
source_filename: hunchsheet-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hunchsheet.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 21:20:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hunchsheet.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hunchsheet-app/security/hunchsheet-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Spreadsheets
- Productivity
- Software-as-a-Service
- Automation
- Company
---
