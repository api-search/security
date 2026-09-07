---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Authentication API
  slug: dremio-intelligent-lakehouse-platform-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Catalog API
  slug: dremio-intelligent-lakehouse-platform-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Jobs API
  slug: dremio-intelligent-lakehouse-platform-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform PAT API
  slug: dremio-intelligent-lakehouse-platform-pat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Reflections API
  slug: dremio-intelligent-lakehouse-platform-reflections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Roles API
  slug: dremio-intelligent-lakehouse-platform-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Scripts API
  slug: dremio-intelligent-lakehouse-platform-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Sources API
  slug: dremio-intelligent-lakehouse-platform-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Dremio Intelligent Lakehouse Platform Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- tokenExchange
overview: Dremio | Intelligent Lakehouse Platform secures its APIs with http and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and tokenExchange flow(s).
provider_name: Dremio | Intelligent Lakehouse Platform
provider_slug: dremio-intelligent-lakehouse-platform
scheme_count: 6
schemes:
- description: 'Authorization: Bearer <token>, where the token is either a personal access token (PAT) or an OAuth access token. This is the only scheme the repo''s OpenAPI files declare.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
  - openapi/dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
  type: http
- description: A long-lived PAT minted per user in the Dremio console. The token carries that user's permissions. It is the authentication method for the Dremio Developer CLI, the self-hosted MCP server, and the Arrow Flight SQL JDBC/ODBC drivers.
  docs: https://docs.dremio.com/dremio-cloud/api/personal-access-token
  managed_by:
  - listUserTokens
  - createUserToken
  name: personalAccessToken
  scheme: bearer
  type: http
- description: Dremio runs its own OAuth authorization server at https://login.dremio.cloud, discoverable per RFC 8414. Supports client credentials for service users, authorization code with PKCE (S256) and dynamic client registration for MCP clients, and RFC 8693 token exchange for an external OIDC JWT or a PAT.
  flows:
  - flow: clientCredentials
    scopes:
    - dremio.all
    tokenUrl: https://login.dremio.cloud/oauth/token
  - authorizationUrl: https://login.dremio.cloud/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://login.dremio.cloud/oauth/register
    scopes:
    - dremio.all
    - offline_access
    tokenUrl: https://login.dremio.cloud/oauth/token
  - flow: tokenExchange
    scopes:
    - dremio.all
    tokenUrl: https://login.dremio.cloud/oauth/token
  name: dremioOAuth
  see: scopes/dremio-intelligent-lakehouse-platform-scopes.yml
  type: oauth2
- description: POST /apiv2/login with userName + password returns a token. Legacy, self-managed only, and rate limited to 45 requests per second per IP.
  name: usernamePassword
  operation: login
  scheme: basic-equivalent
  status: legacy
  type: http
- description: An OIDC provider (Microsoft Entra ID, Okta, LDAP) can authenticate users, and the resulting JWT can be exchanged for a Dremio access token.
  docs: https://docs.dremio.com/dremio-cloud/api/external-token-providers
  name: externalTokenProvider
  type: openIdConnect
- description: SCIM 2.0 provisioning endpoints (/scim/v2) authenticate the identity provider with header auth.
  docs: https://docs.dremio.com/current/security/authentication/identity-providers/scim
  name: scimHeaderAuth
  scheme: bearer
  type: http
slug: dremio-intelligent-lakehouse-platform-authentication
source_filename: dremio-intelligent-lakehouse-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: openapi/*.yml + Dremio authentication documentation\ndocs:\n- https://docs.dremio.com/dremio-cloud/api/\n- https://docs.dremio.com/dremio-cloud/api/oauth-token\n- https://docs.dremio.com/dremio-cloud/api/personal-access-token\n- https://docs.dremio.com/dremio-cloud/security/authentication/personal-access-token\n- https://docs.dremio.com/current/security/authentication/identity-providers/\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials, authorizationCode, tokenExchange]\n  api_key_in: []\n  recommended: >-\n    Dremio recommends exchanging a personal access token for an OAuth access token before using\n    an API application in production.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization: Bearer <token>, where the token is either a personal access token (PAT) or an\n    OAuth access token. This is the only scheme the repo's OpenAPI\
  \ files declare.\n  sources:\n  - openapi/dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-pat-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-roles-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml\n  - openapi/dremio-intelligent-lakehouse-platform-sources-api-openapi.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: >-\n    A long-lived PAT minted per user in the Dremio console. The token carries that user's\n    permissions. It is the authentication method for the Dremio Developer CLI, the self-hosted\n    MCP server, and the Arrow Flight SQL JDBC/ODBC drivers.\n  managed_by:\n  - listUserTokens\n  - createUserToken\n\
  \  docs: https://docs.dremio.com/dremio-cloud/api/personal-access-token\n- name: dremioOAuth\n  type: oauth2\n  description: >-\n    Dremio runs its own OAuth authorization server at https://login.dremio.cloud, discoverable\n    per RFC 8414. Supports client credentials for service users, authorization code with PKCE\n    (S256) and dynamic client registration for MCP clients, and RFC 8693 token exchange for an\n    external OIDC JWT or a PAT.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.dremio.cloud/oauth/token\n    scopes: [dremio.all]\n  - flow: authorizationCode\n    authorizationUrl: https://login.dremio.cloud/oauth/authorize\n    tokenUrl: https://login.dremio.cloud/oauth/token\n    registrationUrl: https://login.dremio.cloud/oauth/register\n    scopes: [dremio.all, offline_access]\n  - flow: tokenExchange\n    tokenUrl: https://login.dremio.cloud/oauth/token\n    scopes: [dremio.all]\n  see: scopes/dremio-intelligent-lakehouse-platform-scopes.yml\n- name:\
  \ usernamePassword\n  type: http\n  scheme: basic-equivalent\n  description: >-\n    POST /apiv2/login with userName + password returns a token. Legacy, self-managed only, and\n    rate limited to 45 requests per second per IP.\n  operation: login\n  status: legacy\n- name: externalTokenProvider\n  type: openIdConnect\n  description: >-\n    An OIDC provider (Microsoft Entra ID, Okta, LDAP) can authenticate users, and the resulting\n    JWT can be exchanged for a Dremio access token.\n  docs: https://docs.dremio.com/dremio-cloud/api/external-token-providers\n- name: scimHeaderAuth\n  type: http\n  scheme: bearer\n  description: >-\n    SCIM 2.0 provisioning endpoints (/scim/v2) authenticate the identity provider with header\n    auth.\n  docs: https://docs.dremio.com/current/security/authentication/identity-providers/scim\nagent_notes: >-\n  Three distinct credentials serve three agent surfaces and they are not interchangeable: the\n  hosted MCP server takes OAuth only, the self-hosted\
  \ MCP server and the CLI take a PAT only, and\n  a service user for machine-to-machine work takes client_id + client_secret. Whatever the\n  credential, authorization is the authenticated principal's RBAC — the OAuth scope is always\n  dremio.all and grants nothing narrower.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/authentication/dremio-intelligent-lakehouse-platform-authentication.yml
summary_line: http/oauth2 · 6 schemes
tags:
- Data
- Analytics
- Lakehouse
- Apache Iceberg
- SQL
- Artificial Intelligence
---
