---
anonymous_access: false
api_key_in:
- query
- header
api_specs:
- filename: first-street-enterprise-api-openapi.yml
  format: yaml
  label: First Street Enterprise API
  slug: first-street-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-enterprise-api-openapi.yml
- filename: first-street-graphql-api-openapi.yml
  format: yaml
  label: First Street Graphql API
  slug: first-street-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-graphql-api-openapi.yml
- filename: first-street-maps-api-openapi.yml
  format: yaml
  label: First Street Maps API
  slug: first-street-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-maps-api-openapi.yml
auth_types:
- apiKey
- http
description: One static API key authenticates every First Street machine surface — REST tiles, both GraphQL endpoints, and the MCP server. There is no OAuth, no OIDC, no token exchange and no scope vocabulary. What replaces scopes is a contractual, per-schema-node entitlement model applied server-side, which is why a valid key can still be refused an individual field.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: First Street Authentication
name_suffix: Authentication
oauth_flows: []
overview: First Street secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: First Street
provider_slug: first-street
scheme_count: 2
schemes:
- applies_to:
  - Climate Risk API
  - Enterprise API
  - Raster Map API
  caution: Query-parameter keys land in access logs, browser history and Referer headers. The docs' own tile-integration guidance requires proxying tile calls server-side so the key is not exposed to a client.
  example: curl "https://api.firststreet.org/v1/apikey?key={api-key}"
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/_original/first-street-openapi.yml
  - docs
  type: apiKey
- applies_to:
  - Climate Risk API
  - Enterprise API
  - Raster Map API
  - MCP server
  example: 'curl "https://api.firststreet.org/v1/apikey" -H "Authorization: Bearer {api-key}"'
  format: Bearer <api-key>
  header: Authorization
  name: bearerAuth
  note: The Bearer shape is borrowed; the credential is a long-lived API key, not an OAuth access token. This is the only accepted form on the MCP server.
  scheme: bearer
  sources:
  - openapi/_original/first-street-openapi.yml
  - docs
  type: http
slug: first-street-authentication
source_filename: first-street-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: https://docs.firststreet.org/api/climate-risk-api/getting-started/authorization\ndocs: https://docs.firststreet.org/api/climate-risk-api/getting-started/authorization\nalso_source:\n  - https://docs.firststreet.org/api/mcp/getting-started\n  - https://docs.firststreet.org/api/enterprise-platform/saml-sso/quickstart\n  - openapi/_original/first-street-openapi.yml\ndescription: >-\n  One static API key authenticates every First Street machine surface — REST tiles,\n  both GraphQL endpoints, and the MCP server. There is no OAuth, no OIDC, no token\n  exchange and no scope vocabulary. What replaces scopes is a contractual, per-schema-node\n  entitlement model applied server-side, which is why a valid key can still be refused an\n  individual field.\n\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  scoped: false\n  human_sso: [saml2]\n\nschemes:\n  - name: apiKeyQuery\n    type: apiKey\n\
  \    in: query\n    parameter: key\n    example: 'curl \"https://api.firststreet.org/v1/apikey?key={api-key}\"'\n    sources: [openapi/_original/first-street-openapi.yml, docs]\n    applies_to: [Climate Risk API, Enterprise API, Raster Map API]\n    caution: >-\n      Query-parameter keys land in access logs, browser history and Referer headers. The\n      docs' own tile-integration guidance requires proxying tile calls server-side so the\n      key is not exposed to a client.\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Bearer <api-key>'\n    example: 'curl \"https://api.firststreet.org/v1/apikey\" -H \"Authorization: Bearer {api-key}\"'\n    sources: [openapi/_original/first-street-openapi.yml, docs]\n    applies_to: [Climate Risk API, Enterprise API, Raster Map API, MCP server]\n    note: >-\n      The Bearer shape is borrowed; the credential is a long-lived API key, not an OAuth\n      access token. This is the only accepted form\
  \ on the MCP server.\n\nmcp:\n  endpoint: https://mcp.firststreet.org/mcp\n  scheme: bearer\n  config_header: '\"Authorization\": \"Bearer <your-token>\"'\n  entitlement: >-\n    \"All API users with access to the Climate Risk API is able utilize First Street's MCP\n    Service\" — no separate MCP credential or consent step.\n  anonymous_surface: >-\n    tools/list answers WITHOUT a key (HTTP 200). Discovery is open; invocation is not.\n\nentitlement_model:\n  granularity: schema node\n  enforced_by: server-side policy directives in the GraphQL schema (@fsHasPolicy, @fsApplyExclusion)\n  evidence: >-\n    The published SDL declares directives `@fsHasPolicy(service: Service!)` and\n    `@fsApplyExclusion` on field definitions — the entitlement machinery is visible in the\n    contract even though the grant matrix is not.\n  failure_mode: >-\n    An unentitled field returns HTTP 200 with that branch null and an \"Error 15: Your\n    account has no access to this node\" entry in errors[].\
  \ See errors/.\n  remediation_contact: api@firststreet.org\n\nkey_management:\n  self_serve: false\n  rotation_policy_published: false\n  guidance:\n    - Do not embed API keys directly in code.\n    - Do not store API keys in files inside your application's source tree.\n    - Set up application and API key restrictions.\n    - Delete unneeded API keys to minimize exposure to attacks.\n    - Regenerate your API keys periodically.\n    - Review your code before publicly releasing it.\n  leak_response: 'Contact your account executive or security@firststreet.org immediately.'\n  note: >-\n    Rate limits and service-specific limits are \"applied during key retrevial\" — the key\n    carries the contract, so keys are not interchangeable between entitlements.\n\nhuman_authentication:\n  surface: First Street Enterprise Suite (https://app.firststreet.org/)\n  method: SAML 2.0 Single Sign-On\n  entity_id: https://auth.firststreet.org/sso/saml/metadata\n  acs_url: https://auth.firststreet.org/sso/saml/acs\n\
  \  metadata: conformance/first-street-saml-sp-metadata.xml\n  attributes: [email, firstName, lastName]\n  attribute_note: Mappings must not be namespaced or prefixed.\n  idp_guides: [Okta, 'Microsoft Entra ID (Azure AD)']\n  setup: account-executive mediated (not self-serve)\n  password_login_after_sso: disabled\n  scim: false\n  scim_note: >-\n    \"First Street currently does not support SCIM.\" User reconciliation is a GraphQL\n    query — rbacGroupUsersConnection(filter: { userGroupId: XX }).\n  docs: https://docs.firststreet.org/api/enterprise-platform/saml-sso/quickstart\n\nnot_supported:\n  - OAuth 2.0 (no authorization server, no /.well-known/oauth-authorization-server)\n  - OpenID Connect (no /.well-known/openid-configuration)\n  - mTLS\n  - Scoped or short-lived API tokens\n  - JWT access tokens\n\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/authentication/first-street-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Climate
- Risk
- Environment
- Modeling
- Geospatial
- Insurance
- Real Estate
- Data
- GraphQL
- Mapping
---
