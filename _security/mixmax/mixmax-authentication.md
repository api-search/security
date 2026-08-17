---
api_key_in:
- header
- query
api_specs:
- filename: mixmax-contact-groups-api-openapi.yml
  format: yaml
  label: Mixmax Contact Groups API
  slug: mixmax-contact-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-contact-groups-api-openapi.yml
- filename: mixmax-contacts-api-openapi.yml
  format: yaml
  label: Mixmax Contacts API
  slug: mixmax-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-contacts-api-openapi.yml
- filename: mixmax-file-requests-api-openapi.yml
  format: yaml
  label: Mixmax File Requests API
  slug: mixmax-file-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-file-requests-api-openapi.yml
- filename: mixmax-meetings-api-openapi.yml
  format: yaml
  label: Mixmax Meetings API
  slug: mixmax-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-meetings-api-openapi.yml
- filename: mixmax-sequences-api-openapi.yml
  format: yaml
  label: Mixmax Sequences API
  slug: mixmax-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-sequences-api-openapi.yml
- filename: mixmax-snippet-tags-api-openapi.yml
  format: yaml
  label: Mixmax Snippet Tags API
  slug: mixmax-snippet-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-snippet-tags-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Mixmax Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- device_code
overview: Mixmax secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code and device_code flow(s).
provider_name: Mixmax
provider_slug: mixmax
scheme_count: 3
schemes:
- alt_in: query
  alt_parameter: apiToken
  description: Mixmax authenticates every REST request with an API token. Create the token under Settings > Integrations (app.mixmax.com/dashboard/settings/personal/integrations); it is displayed only once. Send it as the X-API-Token request header, or as the apiToken query-string parameter.
  in: header
  name: apiToken
  parameter: X-API-Token
  scopes: none
  sources:
  - openapi/mixmax-openapi.yml
  - https://developer.mixmax.com/reference/getting-started-with-the-api
  surface: REST API (https://api.mixmax.com/v1)
  type: apiKey
- authorization_url: https://app.mixmax.com/oidc/auth
  bearer_methods_supported:
  - header
  description: 'The MCP resource server answers an unauthenticated call with 401 and an RFC 9728 challenge — WWW-Authenticate: Bearer resource_metadata="https://mcp.mixmax.com/.well-known/oauth-protected-resource". Clients discover the authorization server from that document, register dynamically, and complete an authorization-code + PKCE flow. Access is read-only.'
  device_code_supported: true
  dynamic_client_registration: true
  flow: authorization_code
  name: mixmaxOAuth
  pkce: S256
  ref: scopes/mixmax-scopes.yml
  registration_url: https://app.mixmax.com/oidc/reg
  revocation_url: https://app.mixmax.com/oidc/token/revocation
  scopes:
  - openid
  - offline_access
  - meetings:read
  sources:
  - https://mcp.mixmax.com/.well-known/oauth-protected-resource
  - https://mcp.mixmax.com/.well-known/oauth-authorization-server
  - https://success.mixmax.com/en/articles/14298142-mixmax-mcp-server
  surface: MCP server (https://mcp.mixmax.com/mcp)
  token_endpoint_auth_methods:
  - none
  token_url: https://app.mixmax.com/oidc/token
  type: oauth2
- description: Mixmax operates its own OpenID Connect provider at https://app.mixmax.com/oidc, with full discovery, JWKS, userinfo, session end and dynamic client registration. It is the authorization server behind the MCP surface.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://app.mixmax.com/oidc
  name: mixmaxOIDC
  openIdConnectUrl: https://app.mixmax.com/oidc/.well-known/openid-configuration
  sources:
  - https://app.mixmax.com/oidc/.well-known/openid-configuration
  subject_types_supported:
  - public
  surface: Mixmax identity provider
  type: openIdConnect
slug: mixmax-authentication
source_filename: mixmax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.mixmax.com/reference/getting-started-with-the-api\ndocs: https://developer.mixmax.com/reference/getting-started-with-the-api\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header, query]\n  oauth2_flows: [authorization_code, device_code]\n  note: >-\n    Mixmax runs two authentication regimes side by side. The classic REST API\n    (https://api.mixmax.com/v1) uses a static per-user API token with no scopes. The newer\n    agent surface — the remote MCP server at https://mcp.mixmax.com/mcp — uses a full OAuth\n    2.0 / OpenID Connect authorization code flow with PKCE against Mixmax's own OIDC provider.\nschemes:\n  - name: apiToken\n    surface: REST API (https://api.mixmax.com/v1)\n    type: apiKey\n    in: header\n    parameter: X-API-Token\n    alt_in: query\n    alt_parameter: apiToken\n    scopes: none\n    description: >-\n      Mixmax authenticates every REST request with an API\
  \ token. Create the token\n      under Settings > Integrations (app.mixmax.com/dashboard/settings/personal/integrations);\n      it is displayed only once. Send it as the X-API-Token request header, or as\n      the apiToken query-string parameter.\n    sources: [openapi/mixmax-openapi.yml, https://developer.mixmax.com/reference/getting-started-with-the-api]\n  - name: mixmaxOAuth\n    surface: MCP server (https://mcp.mixmax.com/mcp)\n    type: oauth2\n    flow: authorization_code\n    pkce: S256\n    dynamic_client_registration: true\n    device_code_supported: true\n    token_endpoint_auth_methods: [none]\n    bearer_methods_supported: [header]\n    authorization_url: https://app.mixmax.com/oidc/auth\n    token_url: https://app.mixmax.com/oidc/token\n    revocation_url: https://app.mixmax.com/oidc/token/revocation\n    registration_url: https://app.mixmax.com/oidc/reg\n    scopes: [openid, offline_access, 'meetings:read']\n    ref: scopes/mixmax-scopes.yml\n    description: >-\n    \
  \  The MCP resource server answers an unauthenticated call with 401 and an RFC 9728\n      challenge — WWW-Authenticate: Bearer resource_metadata=\"https://mcp.mixmax.com/.well-known/oauth-protected-resource\".\n      Clients discover the authorization server from that document, register dynamically,\n      and complete an authorization-code + PKCE flow. Access is read-only.\n    sources:\n      - https://mcp.mixmax.com/.well-known/oauth-protected-resource\n      - https://mcp.mixmax.com/.well-known/oauth-authorization-server\n      - https://success.mixmax.com/en/articles/14298142-mixmax-mcp-server\n  - name: mixmaxOIDC\n    surface: Mixmax identity provider\n    type: openIdConnect\n    openIdConnectUrl: https://app.mixmax.com/oidc/.well-known/openid-configuration\n    issuer: https://app.mixmax.com/oidc\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    description: >-\n      Mixmax operates its own OpenID Connect provider at https://app.mixmax.com/oidc,\
  \ with\n      full discovery, JWKS, userinfo, session end and dynamic client registration. It is the\n      authorization server behind the MCP surface.\n    sources: [https://app.mixmax.com/oidc/.well-known/openid-configuration]\nnotes:\n  - Some REST endpoints (meeting summaries/transcripts) additionally require the workspace-level\n    mixmaxApi feature to be enabled by an admin.\n  - The REST API token is long-lived, unscoped and grants the caller everything the user can do.\n    The MCP surface is the opposite — scoped, revocable, read-only. An integrator choosing\n    between them should know they are not equivalent trust levels.\n  - Message-integration surfaces (Enhancements, Slash Commands, Link Resolvers) are developer-hosted\n    and use their own SDK context rather than either scheme above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/authentication/mixmax-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Saas
- MCP
- Agents
- Webhooks
- OAuth
- Sales Engagement
- Email
- Sales
- CRM
- Productivity
- Meetings
- Sequences
---
