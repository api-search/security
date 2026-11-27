---
api_specs:
- filename: wsystem-dev-billing-api-openapi.yml
  format: yaml
  label: wsystem-dev Billing API
  slug: wsystem-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-billing-api-openapi.yml
- filename: wsystem-dev-company-api-openapi.yml
  format: yaml
  label: wsystem-dev Company API
  slug: wsystem-dev-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-company-api-openapi.yml
- filename: wsystem-dev-e-invoice-api-openapi.yml
  format: yaml
  label: wsystem-dev E Invoice API
  slug: wsystem-dev-e-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-e-invoice-api-openapi.yml
- filename: wsystem-dev-eori-api-openapi.yml
  format: yaml
  label: wsystem-dev EORI API
  slug: wsystem-dev-eori-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-eori-api-openapi.yml
- filename: wsystem-dev-health-api-openapi.yml
  format: yaml
  label: wsystem-dev Health API
  slug: wsystem-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-health-api-openapi.yml
- filename: wsystem-dev-kyb-api-openapi.yml
  format: yaml
  label: wsystem-dev KYB API
  slug: wsystem-dev-kyb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-kyb-api-openapi.yml
- filename: wsystem-dev-sanctions-api-openapi.yml
  format: yaml
  label: wsystem-dev Sanctions API
  slug: wsystem-dev-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-sanctions-api-openapi.yml
- filename: wsystem-dev-vat-api-openapi.yml
  format: yaml
  label: wsystem-dev VAT API
  slug: wsystem-dev-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-vat-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wsystem.dev
  spf: true
hosts:
- cert_expires: Jan 15 09:20:30 2027 GMT
  host: wsystem.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: wsystem-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wsystem-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: wsystem-dev
provider_slug: wsystem-dev
slug: wsystem-dev-domain-security
source_filename: wsystem-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wsystem.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 09:20:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wsystem.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/wsystem-dev/security/wsystem-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Invoicing
- European
- Compliance
---
