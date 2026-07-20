---
api_key_in:
- header
api_specs:
- filename: biodock-public-api-openapi.yml
  format: yaml
  label: Biodock Public API
  slug: biodock-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biodock/refs/heads/main/openapi/biodock-public-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Biodock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biodock secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Biodock
provider_slug: biodock
scheme_count: 1
schemes:
- description: Single API key passed in the X-API-KEY request header on every request. Keys are generated in the Biodock app under Settings -> API (https://app.biodock.ai/settings/api). A key grants access to the owning user's data, so it must be kept secret.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/biodock-public-api-openapi.yml
  type: apiKey
slug: biodock-authentication
source_filename: biodock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.biodock.ai/public-api/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    Single API key passed in the X-API-KEY request header on every request.\n    Keys are generated in the Biodock app under Settings -> API\n    (https://app.biodock.ai/settings/api). A key grants access to the owning\n    user's data, so it must be kept secret.\n  sources: [openapi/biodock-public-api-openapi.yml]\nverify:\n  operation: checkApiKey\n  method: GET\n  url: https://app.biodock.ai/api/external/check\n  note: Returns the user id, email, and a validity message when the key is valid.\nnotes:\n- No OAuth, OpenID Connect, or scoped-permission model is documented; the API\n  uses a single per-user API key.\n- Key management (generate / regenerate) is done in the app UI, not via the API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biodock/refs/heads/main/authentication/biodock-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Image Analysis
- Microscopy
- Life Sciences
- Biotechnology
- Computer Vision
- Cell Analysis
- Research
---
