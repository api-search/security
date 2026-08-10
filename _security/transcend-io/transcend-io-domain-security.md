---
api_specs:
- filename: transcend-io-consent-api-openapi.yml
  format: yaml
  label: Transcend Consent API
  slug: transcend-io-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-consent-api-openapi.yml
- filename: transcend-io-custom-integration-api-openapi.yml
  format: yaml
  label: Transcend Custom Integration API
  slug: transcend-io-custom-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-custom-integration-api-openapi.yml
- filename: transcend-io-data-subject-request-api-openapi.yml
  format: yaml
  label: Transcend Data Subject Request API
  slug: transcend-io-data-subject-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-data-subject-request-api-openapi.yml
- filename: transcend-io-llm-classifier-api-openapi.yml
  format: yaml
  label: Transcend LLM Classifier API
  slug: transcend-io-llm-classifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-llm-classifier-api-openapi.yml
- filename: transcend-io-preferences-api-openapi.yml
  format: yaml
  label: Transcend Preferences API
  slug: transcend-io-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-preferences-api-openapi.yml
- filename: transcend-io-preflight-api-openapi.yml
  format: yaml
  label: Transcend Preflight API
  slug: transcend-io-preflight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-preflight-api-openapi.yml
- filename: transcend-io-public-keys-api-openapi.yml
  format: yaml
  label: Transcend Public Keys API
  slug: transcend-io-public-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-public-keys-api-openapi.yml
- filename: transcend-io-transcend-api-api-openapi.yml
  format: yaml
  label: Transcend Transcend API API
  slug: transcend-io-transcend-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/openapi/transcend-io-transcend-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transcend.io
  spf: true
hosts:
- cert_expires: Sep 15 02:36:24 2026 GMT
  host: transcend.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 01:25:34 2026 GMT
  host: docs.transcend.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.transcend.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transcend Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transcend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transcend
provider_slug: transcend-io
slug: transcend-io-domain-security
source_filename: transcend-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:36:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.transcend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 01:25:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.transcend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: transcend.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/security/transcend-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transcend
- Privacy
- Data Governance
- Consent
- Preference Management
- DSR
- Data Inventory
- AI Governance
- GDPR
- CCPA
- Compliance
- Webhooks
- GraphQL
- MCP
- SDK
- Terraform
- Helm
---
