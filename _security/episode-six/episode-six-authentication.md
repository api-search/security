---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Episode Six Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Episode Six secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Episode Six
provider_slug: episode-six
scheme_count: 1
schemes:
- applies_to: https://docs.episodesix.com/mcp
  dynamic_client_registration:
    registration_endpoint: https://docs.episodesix.com/mcp/oauth/register
    standard: RFC 7591
    supported: true
  flows:
  - authorizationUrl: https://docs.episodesix.com/mcp/oauth/authorize
    flow: authorizationCode
    scopes:
    - mcp:search
    tokenUrl: https://docs.episodesix.com/mcp/oauth/token
  - flow: clientCredentials
    scopes:
    - mcp:search
    tokenUrl: https://docs.episodesix.com/mcp/oauth/token
  issuer: https://docs.episodesix.com/mcp/oauth
  name: MCPOAuth2
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  refresh_supported: true
  response_types:
  - code
  sources:
  - well-known/episode-six-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: episode-six-authentication
source_filename: episode-six-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://docs.episodesix.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Episode Six publishes no public authentication reference. The TRITIUM platform API's auth\n  model (key vs. OAuth vs. mTLS) is documented only inside docs.episodesix.com, which is\n  behind an access-code gate. Nothing is asserted about it here.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  covers:\n  - episode-six-docs-mcp\n  does_not_cover:\n  - episode-six-tritium-platform-api\nschemes:\n- name: MCPOAuth2\n  type: oauth2\n  applies_to: https://docs.episodesix.com/mcp\n  sources:\n  - well-known/episode-six-oauth-authorization-server.json\n  issuer: https://docs.episodesix.com/mcp/oauth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docs.episodesix.com/mcp/oauth/authorize\n    tokenUrl: https://docs.episodesix.com/mcp/oauth/token\n    scopes:\n\
  \    - mcp:search\n  - flow: clientCredentials\n    tokenUrl: https://docs.episodesix.com/mcp/oauth/token\n    scopes:\n    - mcp:search\n  refresh_supported: true\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  dynamic_client_registration:\n    supported: true\n    standard: RFC 7591\n    registration_endpoint: https://docs.episodesix.com/mcp/oauth/register\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  response_types:\n  - code\ngaps:\n- id: tritium-auth-undocumented\n  detail: >-\n    The production TRITIUM platform API authentication model is not publicly documented. An\n    integrator cannot determine the credential type, header, or token lifetime before\n    completing the access-request form.\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://docs.episodesix.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/episode-six/refs/heads/main/authentication/episode-six-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Card Issuing
- Issuer Processing
- Ledger
- Banking
- Financial-Services
- Embedded Finance
- Fintech
- Virtual Accounts
- Virtual Cards
- Credit
- Prepaid
- Multi-Currency
---
