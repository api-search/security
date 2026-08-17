---
api_key_in:
- header
api_specs:
- filename: return-path-everest-api-openapi.yml
  format: yaml
  label: Everest API
  slug: everest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-everest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Return Path Authentication
name_suffix: Authentication
oauth_flows: []
overview: Return Path secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Return Path
provider_slug: return-path
scheme_count: 1
schemes:
- description: 'Every API request requires the X-API-KEY header. Validity''s own wording: "Every API request requires the use of the X-API-KEY header, which is located in your account settings."'
  in: header
  name: apiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/return-path-everest-api-openapi.yml
  type: apiKey
slug: return-path-authentication
source_filename: return-path-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.everest.validity.com/\ndocs: https://developer.everest.validity.com/\nnote: >-\n  The Everest API — the surviving API surface of the Return Path platform after\n  Validity's 2019 acquisition — authenticates with a single static API key sent\n  in the X-API-KEY request header. There is no OAuth, no OIDC and no scope\n  surface, so scopes/ is intentionally absent. The key is issued from Everest\n  account settings; parent accounts can mint child-account keys through the API\n  itself.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    Every API request requires the X-API-KEY header. Validity's own wording:\n    \"Every API request requires the use of the X-API-KEY header, which is\n    located in your account settings.\"\n  sources: [openapi/return-path-everest-api-openapi.yml]\n\
  key_management:\n  self_service: true\n  issued_from: Everest account settings\n  child_keys:\n    supported: true\n    operations:\n    - accountServicesCreateChildAPIKey\n    - apiKeysAPIKeys\n    - apiKeysCreateAPIKey\n    - apiKeysUpdateAPIKey\n    - apiKeysDeleteAPIKey\n  note: >-\n    The API exposes its own key lifecycle — /2.0/accounts/{accountId}/keys\n    lists, creates, updates and deletes keys — so key rotation is programmable.\nobserved:\n  probe: https://api.everest.validity.com/api/2.0/reputation/senderscore/1.1.1.1\n  http_status: 401\n  body: '{\"status\":\"Unauthorized: no valid API credentials provided.\"}'\n  fetched: '2026-08-13'\n  note: >-\n    Probed anonymously. The API answers a clean JSON 401 rather than an HTML\n    error page, which confirms both the auth model and the error envelope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/authentication/return-path-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Martech
- Email
- Email Deliverability
- Email Marketing
- Sender Reputation
- Inbox Placement
- Deliverability
- DMARC
- Email Authentication
- Email Validation
- Analytics
---
