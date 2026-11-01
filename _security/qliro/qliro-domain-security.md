---
api_specs:
- filename: qliro-backwardscompatibilitycheck-api-openapi.yml
  format: yaml
  label: Qliro Backwards Compatibility Check API
  slug: qliro-backwardscompatibilitycheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-backwardscompatibilitycheck-api-openapi.yml
- filename: qliro-creditcheckinformation-api-openapi.yml
  format: yaml
  label: Qliro Credit Check Information API
  slug: qliro-creditcheckinformation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-creditcheckinformation-api-openapi.yml
- filename: qliro-instore-api-openapi.yml
  format: yaml
  label: Qliro In Store API
  slug: qliro-instore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-instore-api-openapi.yml
- filename: qliro-merchantcreditcard-api-openapi.yml
  format: yaml
  label: Qliro Merchant Credit Card API
  slug: qliro-merchantcreditcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-merchantcreditcard-api-openapi.yml
- filename: qliro-paymentoptions-api-openapi.yml
  format: yaml
  label: Qliro Payment Options API
  slug: qliro-paymentoptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-paymentoptions-api-openapi.yml
- filename: qliro-paymentwidget-api-openapi.yml
  format: yaml
  label: Qliro Payment Widget API
  slug: qliro-paymentwidget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-paymentwidget-api-openapi.yml
- filename: qliro-upsell-api-openapi.yml
  format: yaml
  label: Qliro Upsell API
  slug: qliro-upsell-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qliro/openapi/qliro-upsell-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qliro.com
  spf: true
hosts:
- cert_expires: Jan 12 04:11:50 2027 GMT
  host: qliro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qliro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qliro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qliro
provider_slug: qliro
slug: qliro-domain-security
source_filename: qliro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qliro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 04:11:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qliro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/qliro/security/qliro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Buy Now Pay Later
- E-Commerce
---
