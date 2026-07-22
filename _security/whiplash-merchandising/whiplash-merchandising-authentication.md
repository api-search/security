---
api_key_in: []
api_specs:
- filename: whiplash-merchandising-openapi-original.json
  format: json
  label: Rydership API V2
  slug: rydership-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash-merchandising/refs/heads/main/openapi/whiplash-merchandising-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Whiplash Merchandising Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Whiplash Merchandising secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Whiplash Merchandising
provider_slug: whiplash-merchandising
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.getwhiplash.com/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    registrationUrl: https://www.getwhiplash.com/oauth/register
    responseTypes:
    - code
    tokenEndpointAuthMethods:
    - none
    - client_secret_post
    tokenUrl: https://www.getwhiplash.com/oauth/token
  issuer: https://www.getwhiplash.com
  name: OAuth2
  source: https://www.getwhiplash.com/.well-known/oauth-authorization-server
  type: oauth2
slug: whiplash-merchandising-authentication
source_filename: whiplash-merchandising-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.getwhiplash.com/.well-known/oauth-authorization-server\ndocs: https://developers.getwhiplash.com\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  notes: >-\n    The published OpenAPI (Rydership V2) does not declare securitySchemes, but\n    every operation returns 401 unauthorized / 403 forbidden and the live\n    RFC 8414 OAuth Authorization Server Metadata document confirms OAuth 2.0.\n    API access is invite-only (request form via help.whiplash.com).\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://www.getwhiplash.com/.well-known/oauth-authorization-server\n  issuer: https://www.getwhiplash.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.getwhiplash.com/oauth/authorize\n    tokenUrl: https://www.getwhiplash.com/oauth/token\n    registrationUrl: https://www.getwhiplash.com/oauth/register\n    responseTypes: [code]\n    grantTypes: [authorization_code,\
  \ refresh_token]\n    codeChallengeMethods: [S256]\n    tokenEndpointAuthMethods: [none, client_secret_post]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whiplash-merchandising/refs/heads/main/authentication/whiplash-merchandising-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fulfillment
- Logistics
- Ecommerce
- Shipping
- Warehousing
- Inventory
- 3PL
- Order Management
- Returns
- Supply Chain
---
