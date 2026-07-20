---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lingvist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lingvist secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lingvist
provider_slug: lingvist
scheme_count: 1
schemes:
- client_registration: partner-arranged
  flows:
  - authorizationUrl: https://learn.lingvist.com/#sso
    flow: authorizationCode
    scopes:
      auth: Authenticate the user and read their Lingvist profile
    tokenUrl: https://api.lingvist.com/oauth2/token
  name: LingvistOAuth2
  sources:
  - https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/README.md
  - https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/library.js
  token_format: JWT
  token_notes: The plugin decodes the access token with `jws.decode`, confirming the access token is a signed JWT. Profile is retrieved by presenting the access token as an HTTP Bearer credential to the userinfo endpoint.
  token_type: Bearer
  type: oauth2
  userinfo_endpoint: https://api.lingvist.com/1.0/user/profile
slug: lingvist-authentication
source_filename: lingvist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/README.md\ndocs: https://github.com/lingvist/nodebb-plugin-sso-lingvist\nnotes: >-\n  Lingvist publishes no self-serve developer portal or public API documentation.\n  The authentication model below is reconstructed from Lingvist's own first-party\n  open-source NodeBB SSO plugin (github.com/lingvist, npm maintainer \"lingvist\"),\n  whose README documents the production OAuth 2.0 endpoints, and from live probes\n  of those endpoints. OAuth client credentials are \"pre-agreed with Lingvist OAuth\n  provider\" per the README — this is a partner/pre-arranged client program, not\n  self-serve registration.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  token_format: JWT\n  bearer: true\nschemes:\n- name: LingvistOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://learn.lingvist.com/#sso\n\
  \    tokenUrl: https://api.lingvist.com/oauth2/token\n    scopes:\n      auth: Authenticate the user and read their Lingvist profile\n  token_type: Bearer\n  token_format: JWT\n  token_notes: >-\n    The plugin decodes the access token with `jws.decode`, confirming the access\n    token is a signed JWT. Profile is retrieved by presenting the access token as\n    an HTTP Bearer credential to the userinfo endpoint.\n  userinfo_endpoint: https://api.lingvist.com/1.0/user/profile\n  client_registration: partner-arranged\n  sources:\n  - https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/README.md\n  - https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/library.js\nprobes:\n- url: https://api.lingvist.com/oauth2/token\n  method: POST\n  status: 400\n  body: '{\"error\": \"invalid_request\"}'\n  note: RFC 6749 §5.2 error response shape; endpoint is live and POST-only (GET returns 405)\n  probed: '2026-07-19'\n- url: https://api.lingvist.com/1.0/user/profile\n \
  \ method: GET\n  status: 401\n  body: '{\"code\": \"unauthorized\", \"message\": \"Authorization required\"}'\n  note: endpoint is live and requires a bearer credential\n  probed: '2026-07-19'\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  note: >-\n    No RFC 8414 / OIDC discovery document is published on lingvist.com,\n    api.lingvist.com or learn.lingvist.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingvist/refs/heads/main/authentication/lingvist-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Education
- Language Learning
- EdTech
- Artificial Intelligence
- Machine Learning
- Spaced Repetition
- Mobile
- Estonia
- Consumer
---
