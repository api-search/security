---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rephraseai Authentication
name_suffix: Authentication
oauth_flows:
- refreshToken
overview: Rephrase.ai secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the refreshToken flow(s).
provider_name: Rephrase.ai
provider_slug: rephraseai
scheme_count: 1
schemes:
- access_token:
    header: 'Authorization: Bearer <access_token>'
    lifetime_hours: 24
  default_scope: all:diy
  description: 'OAuth2 token exchange. Clients obtain a client_id and refresh_token by contacting Rephrase support, then exchange them for a short-lived access token. All non-auth API calls require the header `Authorization: Bearer <access_token>`.'
  grant_type: refresh_token
  name: RephraseStudioOAuth2
  provisioning: Contact Rephrase support to obtain client_id and refresh_token.
  request_body_fields:
  - default: refresh_token
    name: grant_type
  - description: Provided by Rephrase support
    name: client_id
  - default: all:diy
    name: scope
  - description: Provided by Rephrase support
    name: refresh_token
  sources:
  - https://studio-rephrase-api.readme.io/reference/get-access-token
  token_url: https://auth.rephrase.ai/oauth/token
  type: oauth2
slug: rephraseai-authentication
source_filename: rephraseai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://studio-rephrase-api.readme.io/reference/get-access-token\ndocs: https://studio-rephrase-api.readme.io/reference/documentation\nnote: >-\n  Rephrase.ai was acquired by Adobe in November 2023. The standalone product\n  hosts (rephrase.ai, studio.rephrase.ai, auth.rephrase.ai, api.rephrase.ai) no\n  longer serve TLS and appear decommissioned. This authentication profile is\n  captured from the legacy Rephrase Studio API reference, which is still hosted\n  on ReadMe and remains the only live public surface.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [refreshToken]\n  token_type: bearer\nschemes:\n  - name: RephraseStudioOAuth2\n    type: oauth2\n    description: >-\n      OAuth2 token exchange. Clients obtain a client_id and refresh_token by\n      contacting Rephrase support, then exchange them for a short-lived access\n      token. All non-auth API calls require the header\n      `Authorization: Bearer <access_token>`.\n\
  \    token_url: https://auth.rephrase.ai/oauth/token\n    grant_type: refresh_token\n    default_scope: all:diy\n    request_body_fields:\n      - name: grant_type\n        default: refresh_token\n      - name: client_id\n        description: Provided by Rephrase support\n      - name: scope\n        default: all:diy\n      - name: refresh_token\n        description: Provided by Rephrase support\n    access_token:\n      header: 'Authorization: Bearer <access_token>'\n      lifetime_hours: 24\n    provisioning: Contact Rephrase support to obtain client_id and refresh_token.\n    sources: [https://studio-rephrase-api.readme.io/reference/get-access-token]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/authentication/rephraseai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video
- Text to Video
- Avatars
- Media
- Content Creation
---
