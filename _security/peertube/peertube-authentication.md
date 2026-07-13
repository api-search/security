---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: PeerTube REST API
  slug: peertube-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Chocobozzz/PeerTube/develop/support/doc/api/openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Peertube Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: PeerTube secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: PeerTube
provider_slug: peertube
scheme_count: 1
schemes:
- description: 'Authenticating via OAuth requires the following steps:

    - Have an activated account

    - [Generate] an access token for that account at `/api/v1/users/token`.

    - Make requests with the *Authorization: Bearer <token\>* header

    - Profit, depending on the role assigned to the account


    Note that the __access token is valid for 1 day__ and is given

    along with a __refresh token valid for 2 weeks__.


    [Generate'
  flows:
  - flow: password
    scopes: 3
    tokenUrl: /api/v1/users/token
  name: OAuth2
  sources:
  - openapi/openapi.json
  - openapi/openapi.yaml
  type: oauth2
slug: peertube-authentication
source_filename: peertube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json, openapi/openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/v1/users/token\n    scopes: 3\n  description: |-\n    Authenticating via OAuth requires the following steps:\n    - Have an activated account\n    - [Generate] an access token for that account at `/api/v1/users/token`.\n    - Make requests with the *Authorization: Bearer <token\\>* header\n    - Profit, depending on the role assigned to the account\n\n    Note that the __access token is valid for 1 day__ and is given\n    along with a __refresh token valid for 2 weeks__.\n\n    [Generate\n  sources:\n  - openapi/openapi.json\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peertube/refs/heads/main/authentication/peertube-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Video
- Decentralized
- Federation
- Open Source
- ActivityPub
- Self-Hosted
- Streaming
---
