---
api_specs:
- filename: uetr-ai-account-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Account API
  slug: uetr-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-account-api-openapi.yml
- filename: uetr-ai-owner-confirmation-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Owner confirmation API
  slug: uetr-ai-owner-confirmation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-owner-confirmation-api-openapi.yml
- filename: uetr-ai-payment-records-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Payment records API
  slug: uetr-ai-payment-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-payment-records-api-openapi.yml
- filename: uetr-ai-team-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Team API
  slug: uetr-ai-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-team-api-openapi.yml
- filename: uetr-ai-transfers-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Transfers API
  slug: uetr-ai-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-transfers-api-openapi.yml
- filename: uetr-ai-webhooks-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Webhooks API
  slug: uetr-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uetr.ai
  spf: true
hosts:
- cert_expires: Dec 20 08:46:49 2026 GMT
  host: uetr.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uetr Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SWIFT UETR Tracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SWIFT UETR Tracker
provider_slug: uetr-ai
slug: uetr-ai-domain-security
source_filename: uetr-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uetr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 08:46:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uetr.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/uetr-ai/security/uetr-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- SWIFT
- Tracking
- Financial Services
---
