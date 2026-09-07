---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cloudchipr-enterprise-api-openapi.yml
  format: yaml
  label: CloudChipr API
  slug: cloudchipr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-enterprise-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cloudchipr Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudChipr secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CloudChipr
provider_slug: cloudchipr
scheme_count: 3
schemes:
- applied_to: all 26 operations (per-operation security, no global security block)
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/cloudchipr-enterprise-api-openapi.yml
  - https://docs.cloudchipr.com/docs/api-keys
  surface: https://api.cloudchipr.com
  type: apiKey
- audience: https://api-bff.cloudchipr.com
  authorization_server: https://auth0.cloudchipr.com
  dynamic_client_registration: https://auth0.cloudchipr.com/oidc/register
  format: Bearer <token>
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  in: header
  issuer: https://auth0.cloudchipr.com/
  jwks_uri: https://auth0.cloudchipr.com/.well-known/jwks.json
  name: OAuth2Bearer
  parameter: Authorization
  pkce: S256
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/cloudchipr-mcp-oauth-protected-resource.json
  - well-known/cloudchipr-auth0-openid-configuration.json
  surface: https://mcp.cloudchipr.com/mcp
  type: oauth2
- env: C8R_TOKEN
  format: Bearer <C8R_TOKEN>
  name: ApiKeyBearer
  note: The same in-app CloudChipr API key, presented as a bearer token to the MCP server for headless/CI clients.
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.cloudchipr.com/docs/cloudchipr-mcp-server
  surface: https://mcp.cloudchipr.com/mcp
  type: http
slug: cloudchipr-authentication
source_filename: cloudchipr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  openapi/cloudchipr-enterprise-api-openapi.yml + https://docs.cloudchipr.com/docs/api-keys +\n  https://docs.cloudchipr.com/docs/cloudchipr-mcp-server +\n  https://mcp.cloudchipr.com/.well-known/oauth-protected-resource +\n  https://auth0.cloudchipr.com/.well-known/openid-configuration\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  surfaces: 2\n  note: >-\n    Two surfaces, two different auth models. The REST Enterprise API is apiKey-only\n    (`x-api-key` header, single securityScheme applied per-operation). The hosted MCP server is\n    OAuth 2.0 against an Auth0 tenant, with an API-key-as-bearer alternative for headless use.\n\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    surface: https://api.cloudchipr.com\n    applied_to: 'all 26 operations (per-operation security, no global security block)'\n    sources:\n      - openapi/cloudchipr-enterprise-api-openapi.yml\n\
  \      - https://docs.cloudchipr.com/docs/api-keys\n  - name: OAuth2Bearer\n    type: oauth2\n    surface: https://mcp.cloudchipr.com/mcp\n    in: header\n    parameter: Authorization\n    format: 'Bearer <token>'\n    authorization_server: https://auth0.cloudchipr.com\n    issuer: https://auth0.cloudchipr.com/\n    audience: https://api-bff.cloudchipr.com\n    scopes: [openid, profile, email, offline_access]\n    pkce: S256\n    grant_types: [authorization_code, refresh_token, client_credentials, urn:ietf:params:oauth:grant-type:device_code]\n    dynamic_client_registration: https://auth0.cloudchipr.com/oidc/register\n    jwks_uri: https://auth0.cloudchipr.com/.well-known/jwks.json\n    sources:\n      - well-known/cloudchipr-mcp-oauth-protected-resource.json\n      - well-known/cloudchipr-auth0-openid-configuration.json\n  - name: ApiKeyBearer\n    type: http\n    scheme: bearer\n    surface: https://mcp.cloudchipr.com/mcp\n    parameter: Authorization\n    format: 'Bearer <C8R_TOKEN>'\n\
  \    env: C8R_TOKEN\n    note: The same in-app CloudChipr API key, presented as a bearer token to the MCP server for headless/CI clients.\n    sources:\n      - https://docs.cloudchipr.com/docs/cloudchipr-mcp-server\n\napi_key_lifecycle:\n  issued_in: CloudChipr app -> Settings -> API Keys\n  docs: https://docs.cloudchipr.com/docs/api-keys\n  docs_last_updated: '2025-10-15'\n  max_keys_per_account: 2\n  expiry: '1 to 365 days (minimum 1 day, maximum 365 days)'\n  expiry_superseded: true\n  expiry_superseded_by: https://cloudchipr.com/blog/product-updates-july-1\n  expiry_superseded_note: >-\n    The 2026-07-01 release notes state \"The expiration requirement has also been removed, giving\n    teams more flexibility in how they manage long-lived API credentials\", and that a \"Last Used\"\n    column was added. The docs page still states a mandatory expiry. The provider has not\n    reconciled the two; both are recorded.\n  rotation_guidance: >-\n    CloudChipr publishes rotation guidance\
  \ in the docs (\"Regularly updating and rotating your API\n    keys ... Consider setting an expiration date that aligns with your security policies\") and\n    secure-storage guidance (\"Treat your API keys as sensitive as Read access to cloud accounts and\n    resources\").\n  documented_access_level: read-only\n  documented_access_contradiction: >-\n    The docs state \"API keys provide read-only access to the Cloudchipr API and your cloud\n    resources\", yet the spec secures three MUTATING operations with the same ApiKey scheme:\n    createDataSource (POST /data-sources, 201), updateCategoryStructure\n    (PUT /dimensions/category-structure, 204) and ingestCustomData (POST /ingest/{destinationId}).\n    Recorded, not resolved. An integrator must confirm write capability empirically.\n\nend_user_authentication:\n  mfa: https://docs.cloudchipr.com/docs/multi-factor-authentication-mfa\n  sso:\n    - provider: Okta\n      docs: https://docs.cloudchipr.com/docs/single-sign-on-sso-using-okta\n\
  \    - provider: Azure AD / Entra ID\n      docs: https://docs.cloudchipr.com/docs/single-sign-on-sso-using-azure\n  entitlement: 'Organization SSO is a Pro-tier-and-above entitlement (https://cloudchipr.com/pricing).'\n\ncloud_account_authentication:\n  model: RBAC / role assumption\n  source: https://docs.cloudchipr.com/docs/security-compliance\n  statement: >-\n    \"Cloudchipr does not use Access Key or Secret Key authentication. Connections with customer\n    accounts are mainly done through Role Based Access Control (RBAC).\"\n  provisioning: >-\n    The first-party Terraform module cloudchipr/connect-c8r/cloudchipr (v1.1.9) provisions the\n    read-only role CloudChipr assumes in a customer account. See packages/cloudchipr-packages.yml.\n  docs:\n    - https://docs.cloudchipr.com/docs/read-only-access-requirements\n    - https://docs.cloudchipr.com/docs/create-custom-roles-and-permissions\n    - https://docs.cloudchipr.com/docs/create-custom-roles-and-permissions-in-sub-accounts\n\
  \nobserved:\n  - url: https://api.cloudchipr.com/\n    status: 401\n    body: empty\n    www_authenticate: none\n    checked: '2026-09-05'\n    note: >-\n      The REST host returns a bare 401 with no body and NO WWW-Authenticate header, so an\n      unauthenticated client gets no machine-readable hint about which scheme to use.\n  - url: https://mcp.cloudchipr.com/mcp\n    status: 401\n    body: '{\"error\":\"unauthorized\",\"message\":\"Bearer token required\"}'\n    www_authenticate: 'Bearer realm=\"cloudchipr\", error=\"invalid_token\", error_description=\"No bearer token provided\"'\n    checked: '2026-09-05'\n    note: >-\n      The MCP host does it properly - a WWW-Authenticate Bearer challenge, which combined with the\n      RFC 9728 protected-resource document is enough for an MCP client to discover the\n      authorization server and self-register without human help.\n\nsee_also:\n  scopes: scopes/cloudchipr-scopes.yml\n  conventions: conventions/cloudchipr-conventions.yml\n\
  \  well_known: well-known/cloudchipr-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/authentication/cloudchipr-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Azure
- Cloud Cost Management
- Cost Optimization
- FinOps
- GCP
- Multi-Cloud
- Resource Cleanup
- Rightsizing
---
