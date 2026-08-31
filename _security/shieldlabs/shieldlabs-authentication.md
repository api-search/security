---
api_key_in: []
api_specs:
- filename: shieldlabs-history-api-api-openapi.yml
  format: yaml
  label: ShieldLabs History API
  slug: shieldlabs-history-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shieldlabs/refs/heads/main/openapi/shieldlabs-history-api-api-openapi.yml
- filename: shieldlabs-management-api-api-openapi.yml
  format: yaml
  label: ShieldLabs Management API
  slug: shieldlabs-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shieldlabs/refs/heads/main/openapi/shieldlabs-management-api-api-openapi.yml
- filename: shieldlabs-shieldlabs-api-api-openapi.yml
  format: yaml
  label: ShieldLabs ShieldLabs API
  slug: shieldlabs-shieldlabs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shieldlabs/refs/heads/main/openapi/shieldlabs-shieldlabs-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Shieldlabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShieldLabs secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ShieldLabs
provider_slug: shieldlabs
scheme_count: 2
schemes:
- applies_to: https://account.shieldlabs.ai/api
  description: 'Private API Key from the dashboard API tab, format `sec_xxx-xxx-xxx`. Sent as `Authorization: Bearer sec_…` to the History API on account.shieldlabs.ai. Free reads — does not consume request balance.'
  name: PrivateApiKey
  scheme: bearer
  sources:
  - openapi/shieldlabs-server-api-openapi.yml
  type: http
- additional_headers:
  - description: The registered domain the credential is scoped to.
    name: X-Shield-Domain
    required: true
  applies_to: https://api.shieldlabs.ai
  description: 'Secret Key (32-char hex) sent as `Authorization: Bearer` together with an `X-Shield-Domain` header naming the registered domain. Authenticates the Management API on api.shieldlabs.ai (profile, balance, billed History path).'
  name: SecretKeyHeader
  scheme: bearer
  sources:
  - openapi/shieldlabs-server-api-openapi.yml
  type: http
slug: shieldlabs-authentication
source_filename: shieldlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: openapi/shieldlabs-server-api-openapi.yml\ndocs: https://docs.shieldlabs.ai/setup/keys\nnote: >-\n  Derived from the provider's OpenAPI securitySchemes, then upgraded from the published keys reference.\n  ShieldLabs issues four distinct credentials per registered domain; only two of them appear in the\n  OpenAPI (the two Server API bearer schemes). The public key and the per-endpoint webhook signing\n  secret are documented but are not OpenAPI security schemes, so they are recorded separately below.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  scheme_count: 2\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: PrivateApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Private API Key from the dashboard API tab, format `sec_xxx-xxx-xxx`. Sent as\n    `Authorization: Bearer sec_…` to the History API on account.shieldlabs.ai. Free reads —\n    does not consume\
  \ request balance.\n  applies_to: https://account.shieldlabs.ai/api\n  sources:\n  - openapi/shieldlabs-server-api-openapi.yml\n- name: SecretKeyHeader\n  type: http\n  scheme: bearer\n  description: >-\n    Secret Key (32-char hex) sent as `Authorization: Bearer` together with an `X-Shield-Domain`\n    header naming the registered domain. Authenticates the Management API on api.shieldlabs.ai\n    (profile, balance, billed History path).\n  additional_headers:\n  - name: X-Shield-Domain\n    required: true\n    description: The registered domain the credential is scoped to.\n  applies_to: https://api.shieldlabs.ai\n  sources:\n  - openapi/shieldlabs-server-api-openapi.yml\nnon_api_credentials:\n- name: Public Key\n  format: 32-char hex\n  transport: query parameter `?publicKey=` on the cdn.shieldlabs.ai snippet URL\n  browser_safe: true\n  description: >-\n    Identifies the domain to the ingest gateway. Accepted only when it matches the domain the page\n    is served from (resolved from\
  \ Origin, Referer or Host), so a lifted key will not work elsewhere.\n  docs: https://docs.shieldlabs.ai/setup/keys\n- name: Webhook signing secret\n  format: whsec_…\n  scope: per registered webhook endpoint\n  browser_safe: false\n  description: >-\n    HMAC-SHA256 key used to verify the `X-Shield-Signature: sha256=<hex>` header over the raw\n    webhook body. Not the Secret Key — a separate secret per endpoint.\n  docs: https://docs.shieldlabs.ai/setup/webhooks\nkey_scoping:\n  per_domain: true\n  rotation: >-\n    Key sets rotate from the dashboard; rotation issues a fresh public key and secret key, shows the\n    new secret in full once, and invalidates the old set immediately.\n  masking: keys are masked in the dashboard after issue\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shieldlabs/refs/heads/main/authentication/shieldlabs-authentication.yml
summary_line: http · 2 schemes
tags:
- fraud-detection
- abuse-prevention
- visitor-identification
- device-fingerprinting
- bot-detection
- vpn-proxy-detection
- risk-scoring
- Identity
- Security
- Webhook
- anti-fraud
- traffic-quality
---
