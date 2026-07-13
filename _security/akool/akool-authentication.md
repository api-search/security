---
api_key_in: []
api_specs:
- filename: akool-openapi.yml
  format: yaml
  label: Akool Talking Avatar API
  slug: akool-talking-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Talking Photo API
  slug: akool-talking-photo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Face Swap API
  slug: akool-face-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Video Translation API
  slug: akool-video-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Image Generation API
  slug: akool-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Live Avatar (Streaming) API
  slug: akool-live-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Akool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akool secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Akool
provider_slug: akool
scheme_count: 2
schemes:
- description: 'Bearer token minted by exchanging a clientId and clientSecret at POST https://openapi.akool.com/api/open/v3/getToken. Passed on each request as `Authorization: Bearer {token}`. Token expiry returns error code 1101.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/akool-openapi.yml
  - https://docs.akool.com/authentication/usage
  type: http
- description: Direct API key passed as the `x-api-key` request header. This is the method Akool recommends because it needs no separate token-generation step. The clientId/clientSecret are issued from the Akool OpenAPI settings once you have an eligible plan.
  in: header
  keyName: x-api-key
  name: apiKeyAuth
  sources:
  - openapi/akool-openapi.yml
  - https://docs.akool.com/authentication/usage
  - https://help.akool.com/integrations/api-token
  type: apiKey
slug: akool-authentication
source_filename: akool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/akool-openapi.yml\nsummary:\n  types:\n  - http\n  - apiKey\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token minted by exchanging a clientId and clientSecret at\n    POST https://openapi.akool.com/api/open/v3/getToken. Passed on each request\n    as `Authorization: Bearer {token}`. Token expiry returns error code 1101.\n  sources:\n  - openapi/akool-openapi.yml\n  - https://docs.akool.com/authentication/usage\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: x-api-key\n  description: >-\n    Direct API key passed as the `x-api-key` request header. This is the method\n    Akool recommends because it needs no separate token-generation step. The\n    clientId/clientSecret are issued from the Akool OpenAPI settings once you\n    have an eligible plan.\n  sources:\n  - openapi/akool-openapi.yml\n  - https://docs.akool.com/authentication/usage\n  - https://help.akool.com/integrations/api-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/authentication/akool-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- AI Avatars
- Video Generation
- AI Video
- Face Swap
- Generative AI
- Talking Avatar
- Video Translation
- Live Avatar
---
