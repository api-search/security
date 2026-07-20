---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Flywire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flywire secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flywire
provider_slug: flywire
scheme_count: 1
schemes:
- description: Per-application API key obtained by registering with Flywire (contact Flywire support). Sent on every request as the X-Authentication-Key header.
  in: header
  name: ApiKeyAuth
  parameter_name: X-Authentication-Key
  registration: Contact Flywire to register an application and receive an API key + Shared Secret.
  sources:
  - docs
  type: apiKey
slug: flywire-authentication
source_filename: flywire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.flywire.com/education/Content/api-basics.htm\nnotes: >-\n  Flywire has no published OpenAPI (the api-platform openapi.json returns 401),\n  so this profile is captured from the developer docs rather than derived. The\n  Payments API authorizes with a single static API key sent in a request header;\n  there is no OAuth/OIDC flow and therefore no scopes artifact. Webhook callbacks\n  are separately authenticated by an HMAC-SHA256 signature computed with a shared\n  secret (see asyncapi/flywire-payments-webhooks.yml).\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-Authentication-Key\n  description: >-\n    Per-application API key obtained by registering with Flywire (contact\n    Flywire support). Sent on every request as the X-Authentication-Key header.\n  registration: Contact Flywire to register an application\
  \ and receive an API key + Shared Secret.\n  sources: [docs]\nwebhook_auth:\n  header: X-Flywire-Digest\n  algorithm: HMAC-SHA256 (base64-encoded hash of the request body + Shared Secret)\n  secret: Shared Secret issued at application registration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flywire/refs/heads/main/authentication/flywire-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Cross-Border Payments
- FinTech
- Education Payments
- Healthcare Payments
- Travel Payments
- B2B Payments
- Checkout
- Webhooks
---
