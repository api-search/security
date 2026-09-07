---
anonymous_access: false
api_key_in: []
api_specs:
- filename: atlassian-compass-compass-rest-api-openapi.json
  format: json
  label: Atlassian Compass REST API
  slug: atlassian-compass-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-compass-rest-api-openapi.json
- filename: atlassian-compass-events-api-openapi.yml
  format: yaml
  label: Atlassian Compass Events API
  slug: atlassian-compass-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-events-api-openapi.yml
- filename: atlassian-compass-metrics-api-openapi.yml
  format: yaml
  label: Atlassian Compass Metrics API
  slug: atlassian-compass-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-metrics-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Atlassian Compass Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Atlassian Compass secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Atlassian Compass
provider_slug: atlassian-compass
scheme_count: 2
schemes:
- authorization_model: 'Atlassian states: "If you are making calls directly against the REST API, authorization is based on the user used in the authentication process." There is no service account and no scope negotiation on this path - the token carries the human''s full access.'
  credential_issuer: https://id.atlassian.com/manage/api-tokens
  description: HTTP Basic with an Atlassian account email as the username and an API token as the password
  header: 'Authorization: Basic base64(email:api_token)'
  mfa_note: Atlassian states API tokens allow authentication even when the organization has two-factor authentication or SAML enabled
  name: basicAuth
  rotation: API tokens can be revoked individually from the Atlassian account token manager
  scheme: basic
  sources:
  - openapi/atlassian-compass-compass-rest-api-openapi.json
  type: http
- authorization_server_metadata: https://auth.atlassian.com/.well-known/oauth-authorization-server
  description: OAuth 2.0 (3LO) for Atlassian Cloud
  device_authorization_endpoint: https://auth.atlassian.com/oauth/device/code
  discovery: https://auth.atlassian.com/.well-known/openid-configuration
  dynamic_client_registration: https://auth.atlassian.com/oidc/register
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  pkce:
  - S256
  revocation_endpoint: https://auth.atlassian.com/oauth/revoke
  scopes_detail: scopes/atlassian-compass-scopes.yml
  sources:
  - openapi/atlassian-compass-events-api-openapi.yml
  - openapi/atlassian-compass-metrics-api-openapi.yml
  type: oauth2
slug: atlassian-compass-authentication
source_filename: atlassian-compass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: 'openapi/atlassian-compass-compass-rest-api-openapi.json plus the provider auth docs: https://developer.atlassian.com/cloud/compass/rest/\n  (Authentication + Authorization sections of the published contract narrative), https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/,\n  https://auth.atlassian.com/.well-known/openid-configuration'\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/atlassian-compass-compass-rest-api-openapi.json\n  description: HTTP Basic with an Atlassian account email as the username and an API token as the password\n  credential_issuer: https://id.atlassian.com/manage/api-tokens\n  authorization_model: 'Atlassian states: \"If you are making calls directly against the REST API, authorization\n    is based on the user used in the authentication\
  \ process.\" There is no service account and no scope\n    negotiation on this path - the token carries the human''s full access.'\n  header: 'Authorization: Basic base64(email:api_token)'\n  rotation: API tokens can be revoked individually from the Atlassian account token manager\n  mfa_note: Atlassian states API tokens allow authentication even when the organization has two-factor\n    authentication or SAML enabled\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 (3LO) for Atlassian Cloud\n  sources:\n  - openapi/atlassian-compass-events-api-openapi.yml\n  - openapi/atlassian-compass-metrics-api-openapi.yml\n  discovery: https://auth.atlassian.com/.well-known/openid-configuration\n  authorization_server_metadata: https://auth.atlassian.com/.well-known/oauth-authorization-server\n  pkce:\n  - S256\n  dynamic_client_registration:\
  \ https://auth.atlassian.com/oidc/register\n  revocation_endpoint: https://auth.atlassian.com/oauth/revoke\n  device_authorization_endpoint: https://auth.atlassian.com/oauth/device/code\n  scopes_detail: scopes/atlassian-compass-scopes.yml\ndocs:\n- https://developer.atlassian.com/cloud/compass/rest/\n- https://developer.atlassian.com/cloud/compass/integrations/get-started-integrating-with-Compass/\nadditional_surfaces:\n- surface: Atlassian Rovo MCP Server\n  endpoint: https://mcp.atlassian.com/v2/mcp\n  method: OAuth 2.1 with dynamic client registration\n  protected_resource_metadata: https://mcp.atlassian.com/.well-known/oauth-protected-resource/v2/mcp\n  registration_endpoint: https://mcp.atlassian.com/v1/register\n  note: Compass access over MCP is OAuth-only; Atlassian states API-token authentication is not supported\n    for the Compass permission groups.\n- surface: Atlassian platform GraphQL API\n  endpoint: https://api.atlassian.com/graphql\n  method: OAuth 2.0 3LO, or HTTP Basic\
  \ with an API token for direct calls\n  note: Atlassian's own Compass event-source walkthrough uses an API token against the GraphQL gateway,\n    so both credential types reach the catalog.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/authentication/atlassian-compass-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Atlassian
- Component Management
- Developer Experience
- Software Catalog
- GraphQL
---
