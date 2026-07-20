---
api_key_in:
- header
api_specs:
- filename: art-openapi.yml
  format: yaml
  label: Artsy Public API
  slug: artsy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/art/refs/heads/main/openapi/art-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Art Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artsy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Artsy
provider_slug: art
scheme_count: 1
schemes:
- description: Application-level token obtained from POST /tokens/xapp_token by exchanging client_id and client_secret. Sent in the X-Xapp-Token request header.
  in: header
  name: XappToken
  parameter: X-Xapp-Token
  sources:
  - openapi/art-openapi.yml
  type: apiKey
slug: art-authentication
source_filename: art-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/art-openapi.yml\ndocs: https://developers.artsy.net/v2/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: xapp-token\n  token_endpoint: https://api.artsy.net/api/tokens/xapp_token\n  grant: client_credentials\n  notes: >-\n    Register an application at developers.artsy.net to obtain a client_id and client_secret,\n    then POST them (form-urlencoded or JSON) to /tokens/xapp_token to receive an xapp_token\n    with an expires_at. Send the token in the X-Xapp-Token header on subsequent requests.\n    This is anonymous application-level access; a separate access_token flow exists for\n    user-scoped access.\nschemes:\n- name: XappToken\n  type: apiKey\n  in: header\n  parameter: X-Xapp-Token\n  description: Application-level token obtained from POST /tokens/xapp_token by exchanging client_id\n    and client_secret. Sent in the X-Xapp-Token request header.\n  sources:\n  - openapi/art-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/art/refs/heads/main/authentication/art-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Art
- Marketplace
- Culture
- Museums
- Galleries
- Auctions
- Media
- Hypermedia
- Company
---
