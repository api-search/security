---
api_key_in:
- query
api_specs:
- filename: stackexchange-api-v2-3.yaml
  format: yaml
  label: Stack Exchange API v2.3
  slug: stack-exchange-api-v23
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-api-v2-3.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Stackexchange Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Stack Exchange secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Stack Exchange
provider_slug: stackexchange
scheme_count: 2
schemes:
- description: 'OAuth 2.0 explicit or implicit flow. Apps register on stackapps.com.

    Read methods do not require auth; write methods require `write_access`.

    `private_info` is needed for /me/notifications, /me/inbox, and similar

    private surfaces. `no_expiry` issues tokens that never expire.'
  flows:
  - authorizationUrl: https://stackoverflow.com/oauth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://stackoverflow.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/stackexchange-api-v2-3.yaml
  type: oauth2
- description: 'Optional app key. Sending a key raises the daily quota from 300 to 10,000

    requests per IP and is the recommended default for any non-trivial client.'
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/stackexchange-api-v2-3.yaml
  type: apiKey
slug: stackexchange-authentication
source_filename: stackexchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackexchange-api-v2-3.yaml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://stackoverflow.com/oauth\n    tokenUrl: https://stackoverflow.com/oauth/access_token\n    scopes: 4\n  description: |-\n    OAuth 2.0 explicit or implicit flow. Apps register on stackapps.com.\n    Read methods do not require auth; write methods require `write_access`.\n    `private_info` is needed for /me/notifications, /me/inbox, and similar\n    private surfaces. `no_expiry` issues tokens that never expire.\n  sources:\n  - openapi/stackexchange-api-v2-3.yaml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: |-\n    Optional app key. Sending a key raises the daily quota from 300 to 10,000\n    requests per IP and is the recommended default for\
  \ any non-trivial client.\n  sources:\n  - openapi/stackexchange-api-v2-3.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/authentication/stackexchange-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Q And A
- Developer Community
- Knowledge Graph
- Stack Overflow
- Stack Exchange
- Reputation
- Tags
- Community
- MCP
- AI Grounding
---
