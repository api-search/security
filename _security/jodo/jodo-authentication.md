---
api_key_in: []
api_specs:
- filename: jodo-webhooks-asyncapi.yml
  format: yaml
  label: Jodo Webhooks
  slug: jodo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/asyncapi/jodo-webhooks-asyncapi.yml
- filename: jodo-configuration-api-openapi.yml
  format: yaml
  label: Jodo Configuration API
  slug: jodo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-configuration-api-openapi.yml
- filename: jodo-flex-api-openapi.yml
  format: yaml
  label: Jodo Flex API
  slug: jodo-flex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-flex-api-openapi.yml
- filename: jodo-pay-api-openapi.yml
  format: yaml
  label: Jodo Pay API
  slug: jodo-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-pay-api-openapi.yml
- filename: jodo-students-api-openapi.yml
  format: yaml
  label: Jodo Students API
  slug: jodo-students-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-students-api-openapi.yml
- filename: jodo-users-api-openapi.yml
  format: yaml
  label: Jodo Users API
  slug: jodo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/openapi/jodo-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Jodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jodo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jodo
provider_slug: jodo
scheme_count: 1
schemes:
- applies_to: all operations
  code_snippet_note: Several reference pages show credentials embedded in the URL userinfo (https://JODO_API_KEY:JODO_API_SECRET@JODO_API_HOST/...). This works but leaks credentials into logs, shell history and proxy traces; the Authorization header form shown elsewhere in the same docs is the safer pattern.
  description: All Jodo APIs are authenticated using HTTP Basic Auth. Jodo shares separate API keys and secrets for the UAT/sandbox and production environments. Applied globally in the spec — every documented operation requires it.
  docs: https://docs.jodo.in/getting-started/authentication/
  format: Basic <base64(api_key:api_secret)>
  header: Authorization
  in: header
  name: basicAuth
  provider_guidance:
  - 'Docs caution: "Do not expose API keys or secrets in browsers, mobile apps, or client-side code."'
  - The Android, React Native and Web platform guides all instruct the integrator to mint the hosted-flow redirect_url from their own backend rather than calling Jodo from client code.
  scheme: basic
  sources:
  - openapi/jodo-integrations-openapi.yml
  - https://docs.jodo.in/getting-started/api-structure/
  type: http
slug: jodo-authentication
source_filename: jodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://docs.jodo.in/getting-started/authentication/\ndocs: https://docs.jodo.in/getting-started/authentication/\nsummary:\n  types:\n  - http\n  model: >-\n    Single-scheme HTTP Basic Auth over TLS. Jodo issues an API key and secret per institute per\n    environment and shares them out-of-band; there is no self-service key provisioning, no OAuth,\n    no OpenID Connect and no scope model. Credentials are institute-wide and environment-scoped —\n    the same pair authorises every documented operation, so there is no least-privilege boundary\n    an integrator can apply within an environment.\n  credential_delivery: out-of-band (shared by Jodo per institute and environment)\n  self_service: false\n  scopes: none\n  token_lifetime: n/a (static credential)\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  format: 'Basic <base64(api_key:api_secret)>'\n  description: >-\n   \
  \ All Jodo APIs are authenticated using HTTP Basic Auth. Jodo shares separate API keys and secrets\n    for the UAT/sandbox and production environments. Applied globally in the spec — every documented\n    operation requires it.\n  docs: https://docs.jodo.in/getting-started/authentication/\n  applies_to: all operations\n  sources:\n  - openapi/jodo-integrations-openapi.yml\n  - https://docs.jodo.in/getting-started/api-structure/\n  provider_guidance:\n  - 'Docs caution: \"Do not expose API keys or secrets in browsers, mobile apps, or client-side code.\"'\n  - >-\n    The Android, React Native and Web platform guides all instruct the integrator to mint the\n    hosted-flow redirect_url from their own backend rather than calling Jodo from client code.\n  code_snippet_note: >-\n    Several reference pages show credentials embedded in the URL userinfo\n    (https://JODO_API_KEY:JODO_API_SECRET@JODO_API_HOST/...). This works but leaks credentials into\n    logs, shell history and proxy traces;\
  \ the Authorization header form shown elsewhere in the same\n    docs is the safer pattern.\nend_user_delegation:\n  mechanism: short-lived access token for Jodo-hosted flows\n  description: >-\n    Separate from API authentication. GET /api/v1/integrations/erp/users/{registration_id}/access_token\n    returns an access_token plus expires_at, used to redirect a parent or student into a Jodo-hosted\n    experience at https://[base_url]/consumer/login-redirect?access_token=<token>. This token\n    authenticates the END USER into Jodo's hosted UI; it is not an API credential and cannot be used\n    against the ERP integration endpoints.\n  docs: https://docs.jodo.in/user/api/get-access-token/\nwebhook_authentication:\n  direction: inbound to the integrator\n  mechanisms:\n  - name: HMAC signature\n    header: X-Jodo-Signature\n    algorithm: HMAC SHA-256 hex digest over the raw request body\n    secret: shared secret_key configured per subscription on POST /api/v1/integrations/erp/webhooks\n\
  \  - name: custom header\n    description: An agreed header_key/header_value pair Jodo sends with webhook requests.\n  - name: source IP allowlist\n    production: [3.6.234.242, 3.111.80.40, 13.232.24.175, 43.204.202.190]\n    uat: [3.108.86.33, 13.127.40.177, 65.0.77.215]\n  docs: https://docs.jodo.in/webhooks/security/\ngaps:\n- No OAuth 2.0 or OpenID Connect surface, therefore no scopes and no delegated third-party access.\n- No documented key rotation procedure, key expiry, or credential lifecycle.\n- No documented mTLS option despite the API carrying payment and lending instructions.\n- >-\n  Basic Auth credentials are institute-wide: an ERP integration that only needs to read configuration\n  holds the same credential that can create payment links and cancel payments.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jodo/refs/heads/main/authentication/jodo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Education
- Fintech
- Fee Collection
- Lending
- India
- Webhook
- ERP Integration
- Financial-Services
---
