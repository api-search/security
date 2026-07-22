---
api_key_in:
- query
- header
auth_types:
- http-basic
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Matterport Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MatterPort secures its APIs with http-basic, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MatterPort
provider_slug: matterport
scheme_count: 3
schemes:
- credential_source: Account settings > Developer Tools > API Tokens
  description: Token ID + Token Secret combined as "TokenID:TokenSecret", base64-encoded, sent as the HTTP Basic Authorization header against https://api.matterport.com/api/models/graph.
  name: API Token (GraphQL)
  scheme: basic
  type: http
  used_by:
  - Model API
  - Account API
  - Import API
  - Property Intelligence API
  - Custom Roles API
- description: SDK key appended to the bootstrap script URL (static.matterport.com/showcase-sdk/bootstrap/<ver>/sdk.es6.js?applicationKey=...) to authorize the embedded Showcase player.
  in: query
  name: SDK Application Key
  parameter: applicationKey
  type: apiKey
  used_by:
  - SDK for Embeds
  - SDK Bundle
  - WebComponent
- description: Newer ES6 SDK bootstrap supports connecting to a space via OAuth (not supported by the legacy window.MP_SDK build).
  flows:
  - authorizationCode
  name: OAuth (SDK connect)
  type: oauth2
  used_by:
  - SDK for Embeds
slug: matterport-authentication
source_filename: matterport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://matterport.github.io/showcase-sdk/\ndocs: https://matterport.github.io/showcase-sdk/models_getstarted.html\nnotes: >-\n  Matterport uses distinct auth models for its two developer surfaces. The GraphQL API\n  family (Model/Account/Import) authenticates with an API Token — a Token ID plus a\n  Token Secret created in account settings — sent over HTTP Basic auth. The Showcase\n  SDK (embeds) authenticates with an application/SDK key passed on the bootstrap\n  script URL; newer SDK versions can also connect to a space via OAuth. No OpenAPI is\n  published, so this profile is search-derived from the developer docs rather than a\n  spec.\nsummary:\n  types: [http-basic, apiKey, oauth2]\n  api_key_in: [query, header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: API Token (GraphQL)\n  type: http\n  scheme: basic\n  used_by: [Model API, Account API, Import API, Property Intelligence API, Custom Roles API]\n  description:\
  \ >-\n    Token ID + Token Secret combined as \"TokenID:TokenSecret\", base64-encoded, sent as\n    the HTTP Basic Authorization header against https://api.matterport.com/api/models/graph.\n  credential_source: Account settings > Developer Tools > API Tokens\n- name: SDK Application Key\n  type: apiKey\n  in: query\n  parameter: applicationKey\n  used_by: [SDK for Embeds, SDK Bundle, WebComponent]\n  description: >-\n    SDK key appended to the bootstrap script URL\n    (static.matterport.com/showcase-sdk/bootstrap/<ver>/sdk.es6.js?applicationKey=...)\n    to authorize the embedded Showcase player.\n- name: OAuth (SDK connect)\n  type: oauth2\n  flows: [authorizationCode]\n  used_by: [SDK for Embeds]\n  description: >-\n    Newer ES6 SDK bootstrap supports connecting to a space via OAuth (not supported by\n    the legacy window.MP_SDK build).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matterport/refs/heads/main/authentication/matterport-authentication.yml
summary_line: http-basic/apiKey/oauth2 · 3 schemes
tags:
- Company
- 3D
- Digital Twin
- Spatial Data
- Real Estate
- Construction
- GraphQL
- SDK
- Computer Vision
- Property Intelligence
---
