---
api_specs:
- filename: hypto-banking-api-openapi.yml
  format: yaml
  label: Hypto Banking API
  slug: hypto-banking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-banking-api-openapi.yml
- filename: hypto-generate-qr-api-openapi.yml
  format: yaml
  label: Hypto Generate QR API
  slug: hypto-generate-qr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-generate-qr-api-openapi.yml
- filename: hypto-payments-api-openapi.yml
  format: yaml
  label: Hypto Payments API
  slug: hypto-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-payments-api-openapi.yml
- filename: hypto-status-api-openapi.yml
  format: yaml
  label: Hypto Status API
  slug: hypto-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-status-api-openapi.yml
- filename: hypto-upi-api-openapi.yml
  format: yaml
  label: Hypto UPI API
  slug: hypto-upi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-upi-api-openapi.yml
- filename: hypto-upi-collections-api-openapi.yml
  format: yaml
  label: Hypto UPI Collections API
  slug: hypto-upi-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-upi-collections-api-openapi.yml
- filename: hypto-webhooks-api-openapi.yml
  format: yaml
  label: Hypto Webhooks API
  slug: hypto-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hypto.in
  spf: true
hosts:
- cert_expires: Apr 15 23:59:59 2027 GMT
  host: hypto.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hypto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hypto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hypto
provider_slug: hypto
slug: hypto-domain-security
source_filename: hypto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hypto.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hypto.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hypto/security/hypto-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Fintech
- Collection
---
