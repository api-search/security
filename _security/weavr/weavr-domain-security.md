---
api_specs:
- filename: weavr-multi-openapi-original.yml
  format: yaml
  label: Weavr Multi Product API
  slug: weavr-multi-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-multi-openapi-original.yml
- filename: weavr-multi-backoffice-openapi-original.yml
  format: yaml
  label: Weavr Multi Product BackOffice API
  slug: weavr-multi-product-backoffice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-multi-backoffice-openapi-original.yml
- filename: weavr-payment-run-openapi-original.yml
  format: yaml
  label: Weavr Embedded Payment Run API
  slug: weavr-embedded-payment-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-payment-run-openapi-original.yml
- filename: weavr-simulator-openapi-original.yml
  format: yaml
  label: Weavr Simulator
  slug: weavr-simulator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-simulator-openapi-original.yml
- filename: weavr-webhooks-openapi-original.yml
  format: yaml
  label: Weavr Webhook
  slug: weavr-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/openapi/weavr-webhooks-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: weavr.io
  spf: true
hosts:
- cert_expires: Oct  3 23:02:30 2026 GMT
  host: www.weavr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 11:54:49 2026 GMT
  host: sandbox.weavr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weavr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weavr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Weavr
provider_slug: weavr
slug: weavr-domain-security
source_filename: weavr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weavr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:02:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.weavr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 11:54:49 2026 GMT\n  hsts: null\ndomains:\n- domain: weavr.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weavr/refs/heads/main/security/weavr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Embedded Finance
- Banking as a Service
- Payments
- Cards
- Fintech
- Accounts
- KYC
- Company
---
