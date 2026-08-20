---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Elium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
- refreshToken
overview: Elium secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, password, and refreshToken flow(s).
provider_name: Elium
provider_slug: elium
scheme_count: 1
schemes:
- applies_to:
  - GraphQL API (https://{platform}.elium.com/graphql)
  - MCP server (https://{platform}.elium.com/services/mcp)
  flows:
  - authorizationUrl: https://{platform}.elium.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://{platform}.elium.com/oauth/token
    scopes:
      apiv1: Full access to the Elium API on behalf of the authenticated user
    tokenUrl: https://{platform}.elium.com/oauth/token
    use: Server-side applications acting for an interactive Elium user.
  - flow: password
    scopes:
      apiv1: Full access to the Elium API on behalf of the authenticated user
    tokenUrl: https://{platform}.elium.com/oauth/token
    use: Backend / unattended operations. The provider's guide directs integrators to create a dedicated user account for this grant rather than reusing a human account.
  - flow: refreshToken
    tokenUrl: https://{platform}.elium.com/oauth/token
    use: Renews the access token; a new access token AND a new refresh token are issued on each renewal.
  name: OAuth2
  source: https://learn.elium.com/en/api/getting_started/authentication
  type: oauth2
slug: elium-authentication
source_filename: elium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://learn.elium.com/en/api/getting_started/authentication\ndocs:\n- https://learn.elium.com/en/api/getting_started/authentication\n- https://learn.elium.com/en/api/getting_started/quick_start\n- https://help.elium.com/en/articles/12767574-mcp\nnote: >-\n  Derived nothing from OpenAPI - Elium publishes no OpenAPI. This profile is read from the provider's own\n  authentication guide. Every URL is per-tenant: Elium runs one platform per subdomain, so the\n  authorization, token and revocation endpoints live on the customer's own {platform}.elium.com host.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, password, refreshToken]\n  scopes: [apiv1]\n  token_type: Bearer\n  api_key_alternative: none\n  api_key_note: >-\n    Elium publishes no API-key or personal-access-token path. Every call is OAuth 2.0 on behalf of a user;\n    server-to-server integrations are documented as a password grant\
  \ against a dedicated service user\n    account.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://learn.elium.com/en/api/getting_started/authentication\n  applies_to:\n  - GraphQL API (https://{platform}.elium.com/graphql)\n  - MCP server (https://{platform}.elium.com/services/mcp)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{platform}.elium.com/oauth/authorize\n    tokenUrl: https://{platform}.elium.com/oauth/token\n    refreshUrl: https://{platform}.elium.com/oauth/token\n    scopes: {apiv1: Full access to the Elium API on behalf of the authenticated user}\n    use: Server-side applications acting for an interactive Elium user.\n  - flow: password\n    tokenUrl: https://{platform}.elium.com/oauth/token\n    scopes: {apiv1: Full access to the Elium API on behalf of the authenticated user}\n    use: >-\n      Backend / unattended operations. The provider's guide directs integrators to create a dedicated user\n      account for this grant rather than\
  \ reusing a human account.\n  - flow: refreshToken\n    tokenUrl: https://{platform}.elium.com/oauth/token\n    use: Renews the access token; a new access token AND a new refresh token are issued on each renewal.\ntokens:\n  type: Bearer\n  header: 'Authorization: Bearer <access_token>'\n  expires_in: 3600\n  expires_in_unit: seconds\n  refresh: supported\n  revocation:\n    endpoint: https://{platform}.elium.com/oauth/revoke\n    method: POST\n    parameters: [token, client_id, client_secret]\n    effect: Revokes the access token and its refresh token immediately.\nclient_registration:\n  mechanism: Connected App\n  where: Security tab of the Elium administration panel\n  requires_role: administrator (system role)\n  fields: [name, redirect URL, trusted flag]\n  trusted_flag_effect: >-\n    A Connected App marked \"trusted\" skips the end-user approval screen, for pre-approved corporate\n    applications.\n  dynamic_client_registration: available on request (documented for the MCP surface)\n\
  \  docs: https://help.elium.com/en/articles/12767574-mcp\nauthorization_model:\n  enforcement: per-user\n  detail: >-\n    Access is always evaluated against the authenticated user's own permissions. For MCP the provider\n    states it plainly: \"Every tool runs with the permissions of the authenticated user, so an assistant\n    can only ever access content that user is already allowed to see in Elium.\"\n  sso:\n    supported: true\n    protocols: [SAML 2.0, OpenID Connect]\n    note: >-\n      Enterprise directory SSO (including ADFS/Microsoft) is documented as a platform control, separate\n      from API authentication. Source https://elium.com/trust/controls.\n  mfa:\n    supported: true\n    graphql_operations: [meActivateTwoFactor, meRemoveTwoFactor]\ngaps:\n- No RFC 8414 authorization-server metadata and no OIDC discovery document are served (see\n  well-known/elium-well-known.yml) - a client cannot discover the endpoints programmatically.\n- A single coarse scope (apiv1) grants\
  \ the whole API; there is no read/write or per-resource scoping.\n- No client-credentials grant is documented, so genuine machine-to-machine access is modelled as a\n  password grant against a service user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elium/refs/heads/main/authentication/elium-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Software-as-a-Service
- Knowledge-Management
- Knowledge Base
- Enterprise Search
- AI Search
- GraphQL
- MCP
- Collaboration
- Documentation
- RAG
- Europe
---
