---
api_key_in: []
api_specs:
- filename: typeface-audiences-api-openapi.yml
  format: yaml
  label: Typeface Audiences API
  slug: typeface-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-audiences-api-openapi.yml
- filename: typeface-authentication-api-openapi.yml
  format: yaml
  label: Typeface Authentication API
  slug: typeface-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-authentication-api-openapi.yml
- filename: typeface-basic-services-api-openapi.yml
  format: yaml
  label: Typeface Basic Services API
  slug: typeface-basic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-basic-services-api-openapi.yml
- filename: typeface-brand-kits-api-openapi.yml
  format: yaml
  label: Typeface Brand Kits API
  slug: typeface-brand-kits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-brand-kits-api-openapi.yml
- filename: typeface-content-generation-api-openapi.yml
  format: yaml
  label: Typeface Content Generation API
  slug: typeface-content-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-generation-api-openapi.yml
- filename: typeface-content-service-api-openapi.yml
  format: yaml
  label: Typeface Content Service API
  slug: typeface-content-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-service-api-openapi.yml
- filename: typeface-digital-assets-api-openapi.yml
  format: yaml
  label: Typeface Digital Assets API
  slug: typeface-digital-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-digital-assets-api-openapi.yml
- filename: typeface-discovery-api-openapi.yml
  format: yaml
  label: Typeface Discovery API
  slug: typeface-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-discovery-api-openapi.yml
- filename: typeface-feeds-api-openapi.yml
  format: yaml
  label: Typeface Feeds API
  slug: typeface-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-feeds-api-openapi.yml
- filename: typeface-profile-service-api-openapi.yml
  format: yaml
  label: Typeface Profile Service API
  slug: typeface-profile-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-profile-service-api-openapi.yml
- filename: typeface-projects-api-openapi.yml
  format: yaml
  label: Typeface Projects API
  slug: typeface-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-projects-api-openapi.yml
- filename: typeface-provisioning-api-openapi.yml
  format: yaml
  label: Typeface Provisioning API
  slug: typeface-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-provisioning-api-openapi.yml
- filename: typeface-provisioning-service-api-openapi.yml
  format: yaml
  label: Typeface Provisioning Service API
  slug: typeface-provisioning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-provisioning-service-api-openapi.yml
- filename: typeface-search-service-api-openapi.yml
  format: yaml
  label: Typeface Search Service API
  slug: typeface-search-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-search-service-api-openapi.yml
- filename: typeface-tag-library-api-openapi.yml
  format: yaml
  label: Typeface Tag Library API
  slug: typeface-tag-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-tag-library-api-openapi.yml
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
- Artificial Intelligence
- Content Generation
- Marketing
- Agents
- Generative AI
- Brand Management
- Enterprise
---
