---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Touchmark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Touchmark secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Touchmark
provider_slug: touchmark
scheme_count: 1
schemes:
- description: 'The api_key is sent as "Authorization: Bearer <api_key>". It is a secret that both authenticates the caller and identifies the application (the product being integrated) - the unit event-type schemas and evals are registered against - so no separate application id is passed. Configured once per client (new Touchmark({ api_key })), one client per backend service. During the private beta keys are provisioned by hand by a Touchmark contact and stored as TOUCHMARK_API_KEY. A missing, wrong, or under-permissioned key surfaces as a TouchmarkError with code "auth" - never retryable, always thrown (it never degrades).'
  header: Authorization
  in: header
  name: api_key
  scheme: Bearer
  sources:
  - https://docs.touchmark.ai/sdk/reference
  - https://docs.touchmark.ai/sdk/errors-and-recovery
  type: apiKey
slug: touchmark-authentication
source_filename: touchmark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.touchmark.ai/sdk/reference\ndocs: https://docs.touchmark.ai/sdk/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: api_key\n    type: apiKey\n    in: header\n    header: Authorization\n    scheme: Bearer\n    description: >-\n      The api_key is sent as \"Authorization: Bearer <api_key>\". It is a\n      secret that both authenticates the caller and identifies the application\n      (the product being integrated) - the unit event-type schemas and evals are\n      registered against - so no separate application id is passed. Configured\n      once per client (new Touchmark({ api_key })), one client per backend\n      service. During the private beta keys are provisioned by hand by a\n      Touchmark contact and stored as TOUCHMARK_API_KEY. A missing, wrong, or\n      under-permissioned key surfaces as a TouchmarkError with code \"auth\" -\n      never retryable,\
  \ always thrown (it never degrades).\n    sources:\n      - https://docs.touchmark.ai/sdk/reference\n      - https://docs.touchmark.ai/sdk/errors-and-recovery\nnotes:\n  - No OAuth2, OIDC, or mutualTLS surface is documented; there is no scopes or\n    permissions reference. OAuth scopes artifact intentionally skipped\n    (key-auth-only provider).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/touchmark/refs/heads/main/authentication/touchmark-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Pricing
- Billing
- Monetization
- Evals
- Usage-Based Billing
- Quality Scoring
---
