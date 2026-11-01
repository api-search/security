---
api_specs:
- filename: grainfinance-co-conversions-api-openapi.yml
  format: yaml
  label: Grain Conversions API
  slug: grainfinance-co-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-conversions-api-openapi.yml
- filename: grainfinance-co-customers-api-openapi.yml
  format: yaml
  label: Grain Customers API
  slug: grainfinance-co-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-customers-api-openapi.yml
- filename: grainfinance-co-dual-hedges-api-openapi.yml
  format: yaml
  label: Grain Dual Hedges API
  slug: grainfinance-co-dual-hedges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-dual-hedges-api-openapi.yml
- filename: grainfinance-co-grain-api-api-openapi.yml
  format: yaml
  label: Grain Grain API
  slug: grainfinance-co-grain-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-grain-api-api-openapi.yml
- filename: grainfinance-co-hedges-api-openapi.yml
  format: yaml
  label: Grain Hedges API
  slug: grainfinance-co-hedges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-hedges-api-openapi.yml
- filename: grainfinance-co-payouts-api-openapi.yml
  format: yaml
  label: Grain Payouts API
  slug: grainfinance-co-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-payouts-api-openapi.yml
- filename: grainfinance-co-pricing-api-openapi.yml
  format: yaml
  label: Grain Pricing API
  slug: grainfinance-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-pricing-api-openapi.yml
- filename: grainfinance-co-vendors-api-openapi.yml
  format: yaml
  label: Grain Vendors API
  slug: grainfinance-co-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-vendors-api-openapi.yml
- filename: grainfinance-co-wallets-api-openapi.yml
  format: yaml
  label: Grain Wallets API
  slug: grainfinance-co-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-wallets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issuewild "starfieldtech.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: grainfinance.co
  spf: true
hosts:
- cert_expires: Jan  3 09:58:27 2027 GMT
  host: www.grainfinance.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grainfinance Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Grain
provider_slug: grainfinance-co
slug: grainfinance-co-domain-security
source_filename: grainfinance-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.grainfinance.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 09:58:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: grainfinance.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/grainfinance-co/security/grainfinance-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fintech
- Payments
- Currency
- API
- Embedded
---
