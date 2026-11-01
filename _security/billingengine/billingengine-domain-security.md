---
api_specs:
- filename: billingengine-customers-api-openapi.yml
  format: yaml
  label: BillingEngine Customers API
  slug: billingengine-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billingengine/openapi/billingengine-customers-api-openapi.yml
- filename: billingengine-invoices-api-openapi.yml
  format: yaml
  label: BillingEngine Invoices API
  slug: billingengine-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billingengine/openapi/billingengine-invoices-api-openapi.yml
- filename: billingengine-payments-api-openapi.yml
  format: yaml
  label: BillingEngine Payments API
  slug: billingengine-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billingengine/openapi/billingengine-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: billingengine.com
  spf: true
hosts:
- cert_expires: Nov 26 22:54:58 2026 GMT
  host: www.billingengine.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billingengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BillingEngine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BillingEngine
provider_slug: billingengine
slug: billingengine-domain-security
source_filename: billingengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.billingengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:54:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: billingengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/billingengine/security/billingengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoicing
- Fintech
- Germany
- Small Business
---
