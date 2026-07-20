---
api_key_in: []
api_specs:
- filename: la-ruche-qui-dit-oui-api-openapi.yml
  format: yaml
  label: The Food Assembly API
  slug: food-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-ruche-qui-dit-oui/refs/heads/main/openapi/la-ruche-qui-dit-oui-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: La Ruche Qui Dit Oui Authentication
name_suffix: Authentication
oauth_flows:
- password
- refresh_token
overview: La Ruche qui dit Oui! secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refresh_token flow(s).
provider_name: La Ruche qui dit Oui!
provider_slug: la-ruche-qui-dit-oui
scheme_count: 1
schemes:
- description: OAuth 2 with the resource-owner password credentials grant and the refresh-token grant. Access tokens are presented as bearer tokens.
  flows:
  - flow: password
    parameters:
    - grant_type (value "password")
    - client_id
    - client_secret
    - username
    - password
    scopes: 0
    tokenUrl: https://api.thefoodassembly.com/oauth/v2/token/
  - flow: refresh_token
    parameters:
    - grant_type (value "refresh_token")
    - refresh_token
    - client_id
    - client_secret
    scopes: 0
    tokenUrl: https://api.thefoodassembly.com/oauth/v2/token/
  name: oauth2
  sources:
  - https://github.com/lrqdo/developer/blob/master/api.md
  - openapi/la-ruche-qui-dit-oui-api-openapi.yml
  - live probe of https://api.thefoodassembly.com
  token:
    challenge_header: 'WWW-Authenticate: Bearer'
    challenge_observed: 2026-07-19 at / and /me/
    documented_lifetime_seconds: 3600
    presentation: 'Authorization: Bearer <access_token>'
    refresh: Every exchange returns a fresh refresh_token; clients must persist the new one and discard the old.
    token_type: bearer
  type: oauth2
slug: la-ruche-qui-dit-oui-authentication
source_filename: la-ruche-qui-dit-oui-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/lrqdo/developer/blob/master/api.md\ndocs: https://github.com/lrqdo/developer\nverified_live: '2026-07-19'\noverview: >-\n  The Food Assembly API authenticates with OAuth 2 bearer tokens issued by the\n  resource-owner password credentials grant, with refresh-token rotation. This\n  profile was read from the provider's own published API Blueprint and confirmed\n  against the live host, which answers 401 with a Bearer challenge. No scopes\n  are published — the documented token response carries \"scope\": null.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  - refresh_token\nschemes:\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2 with the resource-owner password credentials grant and the\n    refresh-token grant. Access tokens are presented as bearer tokens.\n  flows:\n  - flow: password\n    tokenUrl: https://api.thefoodassembly.com/oauth/v2/token/\n    scopes: 0\n    parameters:\n\
  \    - grant_type (value \"password\")\n    - client_id\n    - client_secret\n    - username\n    - password\n  - flow: refresh_token\n    tokenUrl: https://api.thefoodassembly.com/oauth/v2/token/\n    scopes: 0\n    parameters:\n    - grant_type (value \"refresh_token\")\n    - refresh_token\n    - client_id\n    - client_secret\n  token:\n    presentation: 'Authorization: Bearer <access_token>'\n    challenge_header: 'WWW-Authenticate: Bearer'\n    challenge_observed: '2026-07-19 at / and /me/'\n    documented_lifetime_seconds: 3600\n    token_type: bearer\n    refresh: >-\n      Every exchange returns a fresh refresh_token; clients must persist the new\n      one and discard the old.\n  sources:\n  - https://github.com/lrqdo/developer/blob/master/api.md\n  - openapi/la-ruche-qui-dit-oui-api-openapi.yml\n  - live probe of https://api.thefoodassembly.com\nscopes:\n  published: false\n  detail: >-\n    No scope registry is documented and the token response returns\n    \"scope\": null.\
  \ Authorization is all-or-nothing; least privilege cannot be\n    requested or verified. No scopes/ artifact is emitted for this repo because\n    there is nothing to record.\npublic_operations:\n- operation: listDistributionProducts\n  detail: The blueprint marks the distribution product listing as a public route.\ndiscovery:\n  openid_configuration: absent (404 on the API host)\n  oauth_authorization_server_metadata: absent (404 on the API host)\n  introspection_endpoint: none documented\n  revocation_endpoint: none documented\n  registration: >-\n    No self-service developer registration exists. client_id and client_secret\n    are not obtainable through any published portal — the documentation gives no\n    instructions for requesting credentials.\nposture:\n  rfc6749_compliant: true\n  rfc6750_compliant: true\n  rfc9700_compliant: false\n  concerns:\n  - >-\n    The resource-owner password credentials grant is the only documented grant.\n    RFC 9700 (OAuth 2.0 Security BCP) recommends\
  \ against it and OAuth 2.1\n    removes it, because it requires every client to handle the end user's\n    password directly.\n  - No PKCE and no authorization code flow are offered.\n  - No scopes, so tokens cannot be constrained to least privilege.\n  - No token introspection or revocation endpoint is documented.\n  - >-\n    No self-service credential issuance, so the API is effectively closed to new\n    integrators regardless of its documentation being public.\nknown_drift:\n  probed: '2026-07-19'\n  detail: >-\n    POST https://api.thefoodassembly.com/oauth/v2/token/ returned 404 with the\n    generic problemType envelope, while GET /me/ correctly returned 401 with a\n    Bearer challenge. The resource surface is live and gated but the documented\n    token endpoint no longer resolves at its published path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-ruche-qui-dit-oui/refs/heads/main/authentication/la-ruche-qui-dit-oui-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Food
- Agriculture
- Marketplace
- E-Commerce
- Local Food
- Sustainability
- France
---
