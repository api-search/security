---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Olx Authentication
name_suffix: Authentication
oauth_flows: []
overview: OLX secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OLX
provider_slug: olx
scheme_count: 1
schemes:
- authorizationUrl: https://www.olx.pl/oauth/authorize/
  bearerFormat: JWT
  evidence:
  - endpoint: https://www.olx.pl/oauth/authorize/
    note: redirects to OLX account login (authorize)
    status: 301
  - endpoint: https://www.olx.pl/api/open/oauth/token
    note: token endpoint
    rejects GET (POST expected): null
    status: 405
  name: OAuth2
  scheme: bearer
  sources:
  - https://developer.olx.pl/api/doc
  tokenUrl: https://www.olx.pl/api/open/oauth/token
  type: oauth2
slug: olx-authentication
source_filename: olx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.olx.pl/api/doc\ndocs: https://developer.olx.pl/api/doc\nsummary:\n  types: [oauth2]\n  token_type: bearer\n  note: >-\n    OLX Poland Partner API uses OAuth2. Access tokens are presented as Bearer\n    tokens in the Authorization header. OLX announced a migration of access\n    tokens from short (~40 character) opaque tokens to JWT access tokens\n    (up to 4096 characters, typically <=1024).\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: bearer\n  authorizationUrl: https://www.olx.pl/oauth/authorize/\n  tokenUrl: https://www.olx.pl/api/open/oauth/token\n  bearerFormat: JWT\n  evidence:\n  - {endpoint: https://www.olx.pl/oauth/authorize/, status: 301, note: redirects to OLX account login (authorize)}\n  - {endpoint: https://www.olx.pl/api/open/oauth/token, status: 405, note: token endpoint, rejects GET (POST expected)}\n  sources: [https://developer.olx.pl/api/doc]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olx/refs/heads/main/authentication/olx-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Marketplace
- Classifieds
- Ecommerce
- Automotive
- Real Estate
- Partner API
---
