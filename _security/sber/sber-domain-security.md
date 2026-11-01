---
api_specs:
- filename: sber-acceptance-advances-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Acceptance Advances API
  slug: sber-acceptance-advances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-acceptance-advances-api-openapi.yml
- filename: sber-auth-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Auth API
  slug: sber-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-auth-api-openapi.yml
- filename: sber-balance-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Balance API
  slug: sber-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-balance-api-openapi.yml
- filename: sber-client-info-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Client Info API
  slug: sber-client-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-client-info-api-openapi.yml
- filename: sber-embeddings-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Embeddings API
  slug: sber-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-embeddings-api-openapi.yml
- filename: sber-files-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Files API
  slug: sber-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-files-api-openapi.yml
- filename: sber-generic-letters-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Generic Letters API
  slug: sber-generic-letters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-generic-letters-api-openapi.yml
- filename: sber-ic-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Ic API
  slug: sber-ic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-ic-api-openapi.yml
- filename: sber-models-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Models API
  slug: sber-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-models-api-openapi.yml
- filename: sber-oauth-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud OAuth API
  slug: sber-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-oauth-api-openapi.yml
- filename: sber-payment-requests-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Payment Requests API
  slug: sber-payment-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-payment-requests-api-openapi.yml
- filename: sber-payments-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Payments API
  slug: sber-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-payments-api-openapi.yml
- filename: sber-placement-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Placement API
  slug: sber-placement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-placement-api-openapi.yml
- filename: sber-room-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Room API
  slug: sber-room-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-room-api-openapi.yml
- filename: sber-sber-id-sbercloud-api-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Sber ID / SberCloud API
  slug: sber-sber-id-sbercloud-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-sber-id-sbercloud-api-api-openapi.yml
- filename: sber-tokens-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Tokens API
  slug: sber-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-tokens-api-openapi.yml
- filename: sber-chat-completions-api-openapi.yml
  format: yaml
  label: Sber ID / SberCloud Chat Completions API
  slug: sber-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sber/openapi/sber-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sber.ru
  spf: true
hosts:
- cert_expires: Dec 24 20:59:59 2026 GMT
  host: sber.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sber ID / SberCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sber ID / SberCloud
provider_slug: sber
slug: sber-domain-security
source_filename: sber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sber.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sber.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sber/security/sber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Infrastructure
- Computing
- Storage
- Russian
---
