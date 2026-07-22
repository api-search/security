---
api_key_in: []
api_specs:
- filename: typeface-api-openapi.json
  format: json
  label: Typeface API
  slug: typeface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-api-openapi.json
- filename: typeface-content-workflow-openapi.json
  format: json
  label: Typeface Content Workflow API
  slug: typeface-content-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-workflow-openapi.json
- filename: typeface-documents-search-openapi.json
  format: json
  label: Typeface Documents Search API
  slug: typeface-documents-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-documents-search-openapi.json
- filename: typeface-team-users-openapi.json
  format: json
  label: Typeface Team Users API
  slug: typeface-team-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-team-users-openapi.json
auth_types:
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Typeface Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Typeface secures its APIs with http-bearer and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Typeface
provider_slug: typeface
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: All REST APIs (except the token endpoint) require an Authorization Bearer <access_token> header. Tokens are JWTs valid for 60 minutes.
  name: bearerAuth
  scheme: bearer
  type: http
- description: Organization admins create an Application in the Typeface UI to obtain applicationId + applicationSecret. POST grant_type=client_credentials with applicationId, applicationSecret, and tenantId (orgId) to the global endpoint to obtain an access token. The token endpoint must always use the global (Azure) API hostname; subsequent requests use the datacenter hostname where the team is provisioned.
  flow: clientCredentials
  name: applicationCredentials
  tokenUrl: https://api-us.typeface.ai/oauth2/token
  type: oauth2
- authorizationUrl: https://auth-us.typeface.ai/authorize
  description: OAuth 2.1 authorization-code flow with PKCE (per the MCP authentication guidelines) for the Typeface MCP server and MCP APIs, with dynamic client registration and optional SSO connection parameter.
  discoveryUrl: https://api-us.typeface.ai/.well-known/oauth-authorization-server
  flow: authorizationCode
  name: mcpOAuth
  pkce: required
  registrationUrl: https://api-us.typeface.ai/mcp/oauth/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  tokenUrl: https://api-us.typeface.ai/mcp/oauth/token
  type: oauth2
slug: typeface-authentication
source_filename: typeface-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.typeface.ai/docs/bearer-authentication\ndocs:\n  - https://developers.typeface.ai/docs/bearer-authentication\n  - https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\nsummary:\n  types: [http-bearer, oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  token_format: JWT\n  token_lifetime_seconds: 3600\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: All REST APIs (except the token endpoint) require an\n      Authorization Bearer <access_token> header. Tokens are JWTs valid for 60\n      minutes.\n  - name: applicationCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api-us.typeface.ai/oauth2/token\n    description: Organization admins create an Application in the Typeface UI\n      to obtain applicationId + applicationSecret. POST\n      grant_type=client_credentials\
  \ with applicationId, applicationSecret, and\n      tenantId (orgId) to the global endpoint to obtain an access token. The\n      token endpoint must always use the global (Azure) API hostname; subsequent\n      requests use the datacenter hostname where the team is provisioned.\n  - name: mcpOAuth\n    type: oauth2\n    flow: authorizationCode\n    pkce: required\n    authorizationUrl: https://auth-us.typeface.ai/authorize\n    tokenUrl: https://api-us.typeface.ai/mcp/oauth/token\n    registrationUrl: https://api-us.typeface.ai/mcp/oauth/register\n    discoveryUrl: https://api-us.typeface.ai/.well-known/oauth-authorization-server\n    scopes:\n      - openid\n      - profile\n      - email\n      - offline_access\n    description: OAuth 2.1 authorization-code flow with PKCE (per the MCP\n      authentication guidelines) for the Typeface MCP server and MCP APIs, with\n      dynamic client registration and optional SSO connection parameter.\nenterprise_identity:\n  sso: [Microsoft Entra\
  \ ID, Okta]\n  provisioning: SCIM 2.0 automated user provisioning (Entra ID and Okta)\n  docs:\n    - https://developers.typeface.ai/docs/sso-configuration-microsoft-entra-id\n    - https://developers.typeface.ai/docs/sso-configuration-okta\n    - https://developers.typeface.ai/docs/azure-ad-members-scynchronization-scim-provisioning\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/authentication/typeface-authentication.yml
summary_line: http-bearer/oauth2 · 3 schemes
tags:
- Company
- Ai
- Artificial Intelligence
- Content Generation
- Marketing
- Agents
- Generative AI
- Brand Management
- Enterprise
---
