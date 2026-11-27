---
api_specs:
- filename: paytrail-payment-reports-api-openapi.yml
  format: yaml
  label: Paytrail payment reports API
  slug: paytrail-payment-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-payment-reports-api-openapi.yml
- filename: paytrail-payments-api-openapi.yml
  format: yaml
  label: Paytrail Payments API
  slug: paytrail-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-payments-api-openapi.yml
- filename: paytrail-providers-api-openapi.yml
  format: yaml
  label: Paytrail Providers API
  slug: paytrail-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-providers-api-openapi.yml
- filename: paytrail-settlements-api-openapi.yml
  format: yaml
  label: Paytrail Settlements API
  slug: paytrail-settlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-settlements-api-openapi.yml
- filename: paytrail-token-payments-api-openapi.yml
  format: yaml
  label: Paytrail token payments API
  slug: paytrail-token-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-token-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paytrail.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: paytrail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Paytrail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paytrail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paytrail
provider_slug: paytrail
slug: paytrail-domain-security
source_filename: paytrail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paytrail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paytrail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/paytrail/security/paytrail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- E-Commerce
- Omnichannel
- Finland
---
