---
api_specs:
- filename: code402-dev-autonomous-api-openapi.yml
  format: yaml
  label: Code402 Autonomous API
  slug: code402-dev-autonomous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-autonomous-api-openapi.yml
- filename: code402-dev-fx-api-openapi.yml
  format: yaml
  label: Code402 Fx API
  slug: code402-dev-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-fx-api-openapi.yml
- filename: code402-dev-modules-api-openapi.yml
  format: yaml
  label: Code402 Modules API
  slug: code402-dev-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-modules-api-openapi.yml
- filename: code402-dev-multimodal-api-openapi.yml
  format: yaml
  label: Code402 Multimodal API
  slug: code402-dev-multimodal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-multimodal-api-openapi.yml
- filename: code402-dev-quota-api-openapi.yml
  format: yaml
  label: Code402 Quota API
  slug: code402-dev-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-quota-api-openapi.yml
- filename: code402-dev-receipt-api-openapi.yml
  format: yaml
  label: Code402 Receipt API
  slug: code402-dev-receipt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-receipt-api-openapi.yml
- filename: code402-dev-tools-api-openapi.yml
  format: yaml
  label: Code402 Tools API
  slug: code402-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-tools-api-openapi.yml
- filename: code402-dev-webhooks-api-openapi.yml
  format: yaml
  label: Code402 Webhooks API
  slug: code402-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: code402.dev
  spf: true
hosts:
- cert_expires: Jan  5 14:28:38 2027 GMT
  host: code402.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Code402 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code402, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Code402
provider_slug: code402-dev
slug: code402-dev-domain-security
source_filename: code402-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: code402.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 14:28:38 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: code402.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/code402-dev/security/code402-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Reconciliation
- x402
- AI Agents
- Verification
- MCP
- ISO 20022
---
