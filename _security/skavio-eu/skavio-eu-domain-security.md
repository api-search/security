---
api_specs:
- filename: skavio-eu-batch-processing-api-openapi.yml
  format: yaml
  label: skavio-eu Batch processing API
  slug: skavio-eu-batch-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-batch-processing-api-openapi.yml
- filename: skavio-eu-billing-api-openapi.yml
  format: yaml
  label: skavio-eu Billing API
  slug: skavio-eu-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-billing-api-openapi.yml
- filename: skavio-eu-bulk-manifests-api-openapi.yml
  format: yaml
  label: skavio-eu Bulk manifests API
  slug: skavio-eu-bulk-manifests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-bulk-manifests-api-openapi.yml
- filename: skavio-eu-contacts-api-openapi.yml
  format: yaml
  label: skavio-eu Contacts API
  slug: skavio-eu-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-contacts-api-openapi.yml
- filename: skavio-eu-events-api-openapi.yml
  format: yaml
  label: skavio-eu Events API
  slug: skavio-eu-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-events-api-openapi.yml
- filename: skavio-eu-flow-api-openapi.yml
  format: yaml
  label: skavio-eu Flow API
  slug: skavio-eu-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-flow-api-openapi.yml
- filename: skavio-eu-invoices-api-openapi.yml
  format: yaml
  label: skavio-eu Invoices API
  slug: skavio-eu-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-invoices-api-openapi.yml
- filename: skavio-eu-me-api-openapi.yml
  format: yaml
  label: skavio-eu Me API
  slug: skavio-eu-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-me-api-openapi.yml
- filename: skavio-eu-operational-notifications-api-openapi.yml
  format: yaml
  label: skavio-eu Operational notifications API
  slug: skavio-eu-operational-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-operational-notifications-api-openapi.yml
- filename: skavio-eu-paid-web-data-api-openapi.yml
  format: yaml
  label: skavio-eu paid web data API
  slug: skavio-eu-paid-web-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-paid-web-data-api-openapi.yml
- filename: skavio-eu-requests-api-openapi.yml
  format: yaml
  label: skavio-eu Requests API
  slug: skavio-eu-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-requests-api-openapi.yml
- filename: skavio-eu-skavio-accounting-api-openapi.yml
  format: yaml
  label: skavio-eu Skavio Accounting API
  slug: skavio-eu-skavio-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-skavio-accounting-api-openapi.yml
- filename: skavio-eu-skavio-processing-api-api-openapi.yml
  format: yaml
  label: skavio-eu Skavio processing API
  slug: skavio-eu-skavio-processing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-skavio-processing-api-api-openapi.yml
- filename: skavio-eu-usdc-payment-verification-api-openapi.yml
  format: yaml
  label: skavio-eu USDC payment verification API
  slug: skavio-eu-usdc-payment-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-usdc-payment-verification-api-openapi.yml
- filename: skavio-eu-webhooks-api-openapi.yml
  format: yaml
  label: skavio-eu Webhooks API
  slug: skavio-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-webhooks-api-openapi.yml
- filename: skavio-eu-workflow-pipelines-api-openapi.yml
  format: yaml
  label: skavio-eu Workflow pipelines API
  slug: skavio-eu-workflow-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-workflow-pipelines-api-openapi.yml
- filename: skavio-eu-x402-api-openapi.yml
  format: yaml
  label: skavio-eu X402 API
  slug: skavio-eu-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skavio.eu
  spf: true
hosts:
- cert_expires: Dec 26 07:18:27 2026 GMT
  host: skavio.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skavio Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for skavio-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: skavio-eu
provider_slug: skavio-eu
slug: skavio-eu-domain-security
source_filename: skavio-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skavio.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 07:18:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skavio.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/skavio-eu/security/skavio-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BusinessTools
- Document Processing
- Invoice Automation
- Audio Transcription
- Payments
---
