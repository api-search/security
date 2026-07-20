---
api_key_in:
- body
auth_types:
- apiKey
- bearer
description: ''
kind: authentication
layout: security
method: searched
name: Immersive Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immersive Labs secures its APIs with apiKey and bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Immersive Labs
provider_slug: immersive-labs
scheme_count: 2
schemes:
- description: An API key generated in the platform (Settings) yields an Access key and a Secret token. These are POSTed as form fields username={access_key} and password={secret_token} to the public tokens endpoint to obtain an access token.
  name: TokenExchange
  request: curl -X POST -d 'username={access_key}&password={secret_token}' https://api.immersivelabs.online/v1/public/tokens
  token_endpoint: https://api.immersivelabs.online/v1/public/tokens
  type: apiKey
- description: 'The access token returned by the tokens endpoint (UUID format) is sent as an Authorization: Bearer {token} header on subsequent GraphQL requests. Tokens expire 30 minutes after issue and must be re-minted.'
  name: BearerToken
  scheme: bearer
  token_ttl_seconds: 1800
  type: http
slug: immersive-labs-authentication
source_filename: immersive-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://support.immersivelabs.com/hc/en-us/articles/29622787761809-API-Guide\ndocs: https://support.immersivelabs.com/hc/en-us/articles/29622787761809-API-Guide\nsummary:\n  types: [apiKey, bearer]\n  api_key_in: [body]\n  model: >-\n    API access key + secret token exchanged for a short-lived bearer access token.\n    No published OpenAPI securitySchemes (the API is GraphQL); this profile is\n    captured from the provider's API Guide.\nschemes:\n- name: TokenExchange\n  type: apiKey\n  description: >-\n    An API key generated in the platform (Settings) yields an Access key and a\n    Secret token. These are POSTed as form fields username={access_key} and\n    password={secret_token} to the public tokens endpoint to obtain an access token.\n  token_endpoint: https://api.immersivelabs.online/v1/public/tokens\n  request: >-\n    curl -X POST -d 'username={access_key}&password={secret_token}'\n    https://api.immersivelabs.online/v1/public/tokens\n\
  - name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    The access token returned by the tokens endpoint (UUID format) is sent as an\n    Authorization: Bearer {token} header on subsequent GraphQL requests. Tokens\n    expire 30 minutes after issue and must be re-minted.\n  token_ttl_seconds: 1800\nnotes:\n- Both the REST and GraphQL surfaces require API-key authentication.\n- The V1 GraphQL API is no longer actively enhanced; API V2 is the active surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immersive-labs/refs/heads/main/authentication/immersive-labs-authentication.yml
summary_line: apiKey/bearer · 2 schemes
tags:
- Company
- Cybersecurity
- Security Training
- Cyber Resilience
- Workforce Development
- GraphQL
- Security
- Compliance
---
