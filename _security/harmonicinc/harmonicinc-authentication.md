---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Harmonicinc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Harmonic Inc. secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Harmonic Inc.
provider_slug: harmonicinc
scheme_count: 1
schemes:
- description: 'The VOS 360 REST API is protected with OAuth 2.0. Clients obtain an access token via the authorization code grant and present it to the API in the HTTP header as `Authorization: Bearer $access_token`. A new access token is obtained after the previous one expires.'
  flows:
  - flow: authorizationCode
  name: OAuth2
  sources:
  - https://s3-us-west-1.amazonaws.com/vos360-public-api/index.html
  type: oauth2
slug: harmonicinc-authentication
source_filename: harmonicinc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://s3-us-west-1.amazonaws.com/vos360-public-api/index.html\ndocs: https://s3-us-west-1.amazonaws.com/vos360-public-api/index.html\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  token_transport: 'Authorization: Bearer $access_token'\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The VOS 360 REST API is protected with OAuth 2.0. Clients obtain an access\n    token via the authorization code grant and present it to the API in the HTTP\n    header as `Authorization: Bearer $access_token`. A new access token is\n    obtained after the previous one expires.\n  flows:\n  - flow: authorizationCode\n  sources:\n  - https://s3-us-west-1.amazonaws.com/vos360-public-api/index.html\nnotes: >-\n  Documented in the \"Getting Started with the REST API — Using OAuth 2.0 to\n  access VOS REST API\" section of the VOS 360 REST API documentation. Explicit\n  authorization/token endpoint URLs and scope\
  \ list are not published in the\n  public reference; captured verbatim from the docs without fabrication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonicinc/refs/heads/main/authentication/harmonicinc-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Video
- Video Streaming
- Broadband
- Media
- Streaming
- SaaS
- Telecommunications
---
