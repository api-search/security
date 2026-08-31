---
api_key_in: []
api_specs:
- filename: demandbase-activities-management-api-openapi.yml
  format: yaml
  label: Demandbase Activities Management API
  slug: demandbase-activities-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-activities-management-api-openapi.yml
- filename: demandbase-asynchronous-batch-api-api-openapi.yml
  format: yaml
  label: Demandbase Asynchronous (Batch) API
  slug: demandbase-asynchronous-batch-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-asynchronous-batch-api-api-openapi.yml
- filename: demandbase-auth-api-openapi.yml
  format: yaml
  label: Demandbase Auth API
  slug: demandbase-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-auth-api-openapi.yml
- filename: demandbase-company-intent-api-openapi.yml
  format: yaml
  label: Demandbase Company Intent API
  slug: demandbase-company-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-company-intent-api-openapi.yml
- filename: demandbase-create-export-job-api-openapi.yml
  format: yaml
  label: Demandbase Create Export Job API
  slug: demandbase-create-export-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-create-export-job-api-openapi.yml
- filename: demandbase-credit-usage-api-openapi.yml
  format: yaml
  label: Demandbase Credit Usage API
  slug: demandbase-credit-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-credit-usage-api-openapi.yml
- filename: demandbase-custom-sources-api-openapi.yml
  format: yaml
  label: Demandbase Custom Sources API
  slug: demandbase-custom-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-custom-sources-api-openapi.yml
- filename: demandbase-field-mappings-api-openapi.yml
  format: yaml
  label: Demandbase Field Mappings API
  slug: demandbase-field-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-field-mappings-api-openapi.yml
- filename: demandbase-get-fields-api-openapi.yml
  format: yaml
  label: Demandbase Get Fields API
  slug: demandbase-get-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-get-fields-api-openapi.yml
- filename: demandbase-get-job-details-api-openapi.yml
  format: yaml
  label: Demandbase Get Job Details API
  slug: demandbase-get-job-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-get-job-details-api-openapi.yml
- filename: demandbase-get-reference-data-api-openapi.yml
  format: yaml
  label: Demandbase Get Reference Data API
  slug: demandbase-get-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-get-reference-data-api-openapi.yml
- filename: demandbase-import-job-api-openapi.yml
  format: yaml
  label: Demandbase Import Job API
  slug: demandbase-import-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-import-job-api-openapi.yml
- filename: demandbase-reference-tables-api-openapi.yml
  format: yaml
  label: Demandbase Reference Tables API
  slug: demandbase-reference-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-reference-tables-api-openapi.yml
- filename: demandbase-subscription-api-api-openapi.yml
  format: yaml
  label: Demandbase Subscription API
  slug: demandbase-subscription-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-subscription-api-api-openapi.yml
- filename: demandbase-sync-api-api-openapi.yml
  format: yaml
  label: Demandbase Sync API
  slug: demandbase-sync-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-sync-api-api-openapi.yml
- filename: demandbase-user-management-api-openapi.yml
  format: yaml
  label: Demandbase User Management API
  slug: demandbase-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-user-management-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Demandbase Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Demandbase secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Demandbase
provider_slug: demandbase
scheme_count: 1
schemes:
- description: Bearer access token obtained from POST /auth/v1/token. Named `token` in the Admin, Data Export and Auth specs and `bearerAuth` in the B2B, Import, Intent, Usage and Custom Sources specs — the same credential either way.
  docs: https://developer.demandbase.com/docs/auth-api
  name: token
  scheme: bearer
  sources:
  - openapi/demandbase-admin-openapi.yml
  - openapi/demandbase-b2b-openapi.yml
  - openapi/demandbase-custom-sources-openapi.yml
  - openapi/demandbase-data-export-openapi.yml
  - openapi/demandbase-data-import-openapi.yml
  - openapi/demandbase-intent-openapi.yml
  - openapi/demandbase-usage-openapi.yml
  type: http
slug: demandbase-authentication
source_filename: demandbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/*.json (8 harvested Demandbase OpenAPI definitions)\ndocs:\n  - https://developer.demandbase.com/docs/authenticating-with-the-apis\n  - https://developer.demandbase.com/docs/migrating-from-legacy-tokens-to-api-keysets\n  - https://developer.demandbase.com/reference/generate_access_token\n  - https://developer.demandbase.com/docs/custom-mcp-clients\nnote: >-\n  Demandbase runs two distinct authentication models on two distinct surfaces, and they do\n  not share credentials. The REST platform APIs use an OAuth 2.0 client-credentials exchange\n  against its own token endpoint and then a plain HTTP bearer token. The MCP gateway uses a\n  full OAuth 2.1 authorization-code + PKCE flow with dynamic client registration against an\n  Okta-backed authorization server. Both are recorded below.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  api_key_in:\
  \ []\n  mtls: false\n  openid_connect: true\nschemes:\n  - name: token\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer access token obtained from POST /auth/v1/token. Named `token` in the Admin,\n      Data Export and Auth specs and `bearerAuth` in the B2B, Import, Intent, Usage and\n      Custom Sources specs — the same credential either way.\n    sources:\n      - openapi/demandbase-admin-openapi.yml\n      - openapi/demandbase-b2b-openapi.yml\n      - openapi/demandbase-custom-sources-openapi.yml\n      - openapi/demandbase-data-export-openapi.yml\n      - openapi/demandbase-data-import-openapi.yml\n      - openapi/demandbase-intent-openapi.yml\n      - openapi/demandbase-usage-openapi.yml\n    docs: https://developer.demandbase.com/docs/auth-api\ntoken_exchange:\n  endpoint: https://uapi.demandbase.com/auth/v1/token\n  method: POST\n  operation: openapi/demandbase-auth-openapi.yml#POST /auth/v1/token\n  content_type: application/json\n  request:\n    grantType:\
  \ client_credentials\n    clientId: <API Key Set client ID>\n    clientSecret: <API Key Set client secret>\n  response:\n    accessToken: bearer token for authenticated API calls\n    tokenType: bearer\n    expiresIn: 28800\n  usage: 'Authorization: Bearer <access-token>'\n  warning: Do not send the Client Secret directly in the Authorization header.\ncredentials:\n  container: API Key Set\n  scope: >-\n    Platform-level, not user-level. An API Key Set is a named permission container for one\n    integration; permissions are explicitly assigned to it and survive changes to any\n    individual user.\n  management: https://support.demandbase.com/hc/en-us/articles/38999526296603-Generate-and-Manage-API-Key-Sets\n  rotation: >-\n    Demandbase recommends one API Key Set per independent workload or trust boundary so\n    credentials can be rotated per integration.\n  legacy:\n    name: Legacy API token\n    shape: A single user-scoped token sent directly as the bearer token.\n    risk: >-\n\
  \      Because it is tied to an individual user's profile, deactivating that user breaks\n      every integration using the token.\n    migration: https://developer.demandbase.com/docs/migrating-from-legacy-tokens-to-api-keysets\n    sunset_date: null\nmcp_authentication:\n  surface: https://gateway.demandbase.com/mcp/servers/db-mcp\n  scheme: OAuth 2.1 authorization code + PKCE (S256)\n  dynamic_client_registration: true\n  registration_endpoint: https://gateway.demandbase.com/mcp/v1/register\n  issuer: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7\n  authorization_endpoint: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/authorize\n  token_endpoint: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/token\n  token_endpoint_auth_methods_supported: [none]\n  scopes_supported: [openid, profile, email, offline_access]\n  resource: https://gateway.demandbase.com/mcp/\n  protected_resource_metadata: https://gateway.demandbase.com/.well-known/oauth-protected-resource\n\
  \  challenge: >-\n    An unauthenticated request returns HTTP 401 with\n    WWW-Authenticate: Bearer resource_metadata=\"…/.well-known/oauth-protected-resource\",\n    which is the RFC 9728 discovery bootstrap an MCP client needs.\n  guidance: >-\n    Demandbase explicitly instructs clients not to hardcode the authorization or token\n    endpoints, and to key stored registrations and tokens on the discovered issuer.\n  docs: https://developer.demandbase.com/docs/custom-mcp-clients\nidentity_provider:\n  host: authentication.demandbase.com\n  vendor: Okta\n  openid_configuration: well-known/demandbase-auth-openid-configuration.json\n  oauth_authorization_server: well-known/demandbase-auth-oauth-authorization-server.json\nauthorization:\n  model: >-\n    Access is governed by Permission Sets in Demandbase One, including a dedicated MCP tab\n    with Full Access / Limited Access (Demandbase Data and/or Your Data) / No Access. Data\n    Export access is additionally gated by the tenant's Export\
  \ Collection (1-4), which\n    determines which entity types and fields may be requested at all.\n  docs:\n    - https://support.demandbase.com/hc/en-us/articles/4408096198811-Understanding-Permission-Sets\n    - https://developer.demandbase.com/docs/collections\nrelated:\n  - scopes/demandbase-scopes.yml\n  - conventions/demandbase-conventions.yml\n  - well-known/demandbase-well-known.yml\n  - mcp/demandbase-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/authentication/demandbase-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Account-Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Company Data
- Contact Data
- Data Enrichment
- Intent Data
- MCP
- Personalization
- Sales Intelligence
- Technographics
---
