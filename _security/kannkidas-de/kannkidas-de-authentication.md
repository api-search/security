---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kannkidas-de-openapi.yml
  format: yaml
  label: Kann KI das? API
  slug: kann-ki-das-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kannkidas-de/refs/heads/main/openapi/kannkidas-de-openapi.yml
auth_types:
- none
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kannkidas De Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Kann KI das? Sponsoring Agent secures its APIs with none, http, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Kann KI das? Sponsoring Agent
provider_slug: kannkidas-de
scheme_count: 2
schemes:
- applies_to:
  - issueAgentAccessToken
  name: clientBasic
  note: client_id / client_secret from registration, used only at the token endpoint.
  scheme: basic
  sources:
  - openapi/kannkidas-de-openapi.yml
  type: http
- applies_to:
    createSponsorPurchase:
    - sponsorship:write
    getSponsorPurchase:
    - sponsorship:read
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://kannkidas.de/api/oauth/token
  name: oauth2
  sources:
  - openapi/kannkidas-de-openapi.yml
  - https://kannkidas.de/auth.md
  type: oauth2
slug: kannkidas-de-authentication
source_filename: kannkidas-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/kannkidas-de-openapi.yml\ndocs: https://kannkidas.de/auth.md\ndiscovery:\n  oauth_authorization_server: https://kannkidas.de/.well-known/oauth-authorization-server\n  openid_configuration: https://kannkidas.de/.well-known/openid-configuration\n  oauth_protected_resource: https://kannkidas.de/.well-known/oauth-protected-resource\n  jwks_uri: https://kannkidas.de/.well-known/jwks.json (empty key set — tokens are opaque)\n  issuer: https://kannkidas.de\n  resource: https://kannkidas.de/api\nsummary:\n  types:\n  - none\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  anonymous_operations: [searchProductsAndCategories, suggestSearchTerms, getSimilarProducts, listSponsorSlots, registerAgentClient, getPaidSponsorBuyerBrief (x402 402)]\n  registration: anonymous dynamic client registration at POST https://kannkidas.de/api/agent/register (JSON {name 3-80 chars, scopes?}); the client secret is returned exactly\
  \ once.\n  token: POST https://kannkidas.de/api/oauth/token, HTTP Basic (client_secret_basic), grant_type=client_credentials, optional scope (default sponsorship:read); returns a short-lived opaque bearer token (lifetime not stated).\n  bearer_methods_supported: [header]\n  rule: Send tokens only in the Authorization header; never place a client secret or token in a URL (auth.md).\n  agent_auth_extension: The served metadata carries a non-standard agent_auth block (skill https://kannkidas.de/auth.md, identity_types_supported [anonymous], credential_types_supported [oauth_client_credentials]).\nschemes:\n- name: clientBasic\n  type: http\n  scheme: basic\n  applies_to: [issueAgentAccessToken]\n  note: client_id / client_secret from registration, used only at the token endpoint.\n  sources:\n  - openapi/kannkidas-de-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://kannkidas.de/api/oauth/token\n    scopes: 2\n  applies_to:\n    createSponsorPurchase:\
  \ [sponsorship:write]\n    getSponsorPurchase: [sponsorship:read]\n  sources:\n  - openapi/kannkidas-de-openapi.yml\n  - https://kannkidas.de/auth.md\nmcp:\n  endpoint: https://kannkidas.de/api/mcp\n  server_card_authentication: oauth2 with protectedResourceMetadata https://kannkidas.de/.well-known/oauth-protected-resource\n  observed: initialize and tools/list succeed anonymously; create_sponsor_checkout requires sponsorship:write.\na2a:\n  endpoint: https://kannkidas.de/api/a2a\n  observed: anonymous, read-only; the agent card declares no securitySchemes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kannkidas-de/refs/heads/main/authentication/kannkidas-de-authentication.yml
summary_line: none/http/oauth2 · 2 schemes
tags:
- Company
- Sponsoring
- Advertising
- Software Reviews
- Build vs Buy
- Search
- Agent-Native
- MCP
- A2A
- Authentication
- x402
- Stripe Checkout
- Germany
---
