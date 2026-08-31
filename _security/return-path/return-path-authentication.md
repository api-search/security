---
api_key_in:
- header
api_specs:
- filename: return-path-account-services-api-openapi.yml
  format: yaml
  label: Return Path Account Services API
  slug: return-path-account-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-account-services-api-openapi.yml
- filename: return-path-apps-integrations-api-openapi.yml
  format: yaml
  label: Return Path Apps & Integrations API
  slug: return-path-apps-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-apps-integrations-api-openapi.yml
- filename: return-path-certification-api-openapi.yml
  format: yaml
  label: Return Path Certification API
  slug: return-path-certification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-certification-api-openapi.yml
- filename: return-path-competitive-intel-api-openapi.yml
  format: yaml
  label: Return Path Competitive Intel API
  slug: return-path-competitive-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-competitive-intel-api-openapi.yml
- filename: return-path-engagement-api-openapi.yml
  format: yaml
  label: Return Path Engagement API
  slug: return-path-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-engagement-api-openapi.yml
- filename: return-path-inbox-placement-api-openapi.yml
  format: yaml
  label: Return Path Inbox Placement API
  slug: return-path-inbox-placement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-inbox-placement-api-openapi.yml
- filename: return-path-infrastructure-dmarc-api-openapi.yml
  format: yaml
  label: Return Path Infrastructure (DMARC) API
  slug: return-path-infrastructure-dmarc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-infrastructure-dmarc-api-openapi.yml
- filename: return-path-legacy-api-1-0-api-openapi.yml
  format: yaml
  label: Return Path Legacy API (1.0) API
  slug: return-path-legacy-api-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-legacy-api-1-0-api-openapi.yml
- filename: return-path-list-validation-api-openapi.yml
  format: yaml
  label: Return Path List Validation API
  slug: return-path-list-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-list-validation-api-openapi.yml
- filename: return-path-reputation-api-openapi.yml
  format: yaml
  label: Return Path Reputation API
  slug: return-path-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-reputation-api-openapi.yml
- filename: return-path-view-time-optimization-api-openapi.yml
  format: yaml
  label: Return Path View Time Optimization API
  slug: return-path-view-time-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-view-time-optimization-api-openapi.yml
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
- MarTech
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
