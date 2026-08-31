---
api_key_in:
- header
api_specs:
- filename: immuta-access-request-api-openapi.yml
  format: yaml
  label: Immuta Access Request API
  slug: immuta-access-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-access-request-api-openapi.yml
- filename: immuta-asset-api-openapi.yml
  format: yaml
  label: Immuta Asset API
  slug: immuta-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-asset-api-openapi.yml
- filename: immuta-auth-api-openapi.yml
  format: yaml
  label: Immuta Auth API
  slug: immuta-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-auth-api-openapi.yml
- filename: immuta-data-product-api-openapi.yml
  format: yaml
  label: Immuta Data Product API
  slug: immuta-data-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-data-product-api-openapi.yml
- filename: immuta-data-source-api-openapi.yml
  format: yaml
  label: Immuta Data Source API
  slug: immuta-data-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-data-source-api-openapi.yml
- filename: immuta-data-use-agreement-api-openapi.yml
  format: yaml
  label: Immuta Data Use Agreement API
  slug: immuta-data-use-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-data-use-agreement-api-openapi.yml
- filename: immuta-health-api-openapi.yml
  format: yaml
  label: Immuta Health API
  slug: immuta-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-health-api-openapi.yml
- filename: immuta-metadata-api-openapi.yml
  format: yaml
  label: Immuta Metadata API
  slug: immuta-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-metadata-api-openapi.yml
- filename: immuta-notification-api-openapi.yml
  format: yaml
  label: Immuta Notification API
  slug: immuta-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-notification-api-openapi.yml
- filename: immuta-request-form-api-openapi.yml
  format: yaml
  label: Immuta Request Form API
  slug: immuta-request-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-request-form-api-openapi.yml
- filename: immuta-settings-api-openapi.yml
  format: yaml
  label: Immuta Settings API
  slug: immuta-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/openapi/immuta-settings-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Immuta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immuta secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Immuta
provider_slug: immuta
scheme_count: 3
schemes:
- bearerFormat: JWT
  claims_note: the JWT claims carry tenant metadata used to build the Request app request context
  credential: personal access token (PAT)
  expiration: configurable at creation, including "No expiration"
  issued_at: https://app.immutacloud.com/marketplace/personal-access-tokens
  management_operations:
  - createToken
  - listTokens
  - getToken
  - deleteToken
  - user
  name: bearer
  scheme: bearer
  sources:
  - openapi/immuta-marketplace-api-openapi.yml
  surface: Immuta Data Marketplace / Request app API
  type: http
  visibility: shown once at creation and not retrievable afterwards
- in: header
  issued_at: the API Keys tab of the Immuta user profile page
  name: immutaApiKey
  note: 'the API key is sent as the raw Authorization header value with no scheme prefix — Authorization: <api-key>'
  parameter_name: Authorization
  sources:
  - https://documentation.immuta.com/saas/developer-guides/api-intro/authentication
  surface: Immuta Govern API (V1, V2, integrations, connections) and the Immuta CLI
  type: apiKey
- exchange:
    endpoint: POST /bim/apikey/authenticate
    request: '{"apikey": "<your-api-key>"}'
    response: bearer token presented as Authorization Bearer on subsequent calls
  name: immutaBearerExchange
  scheme: bearer
  sources:
  - https://documentation.immuta.com/saas/developer-guides/api-intro/authentication
  surface: Immuta Govern API
  type: http
slug: immuta-authentication
source_filename: immuta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/immuta-marketplace-api-openapi.yml\ndocs: https://documentation.immuta.com/saas/developer-guides/api-intro/authentication\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: 'Immuta''s APIs are key- and token-authenticated, not OAuth-scoped. There is\n    no authorization server, no scope surface and no /.well-known discovery; authorization\n    is enforced by Immuta permissions (for example CREATE_DATA_SOURCE, APPLICATION_ADMIN)\n    attached to the calling identity rather than by token scopes.'\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  surface: Immuta Data Marketplace / Request app API\n  sources: [openapi/immuta-marketplace-api-openapi.yml]\n  credential: personal access token (PAT)\n  issued_at: https://app.immutacloud.com/marketplace/personal-access-tokens\n  expiration: configurable at creation, including \"No expiration\"\n  visibility:\
  \ shown once at creation and not retrievable afterwards\n  claims_note: the JWT claims carry tenant metadata used to build the Request app request\n    context\n  management_operations: [createToken, listTokens, getToken, deleteToken, user]\n- name: immutaApiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  surface: Immuta Govern API (V1, V2, integrations, connections) and the Immuta CLI\n  sources: [https://documentation.immuta.com/saas/developer-guides/api-intro/authentication]\n  note: 'the API key is sent as the raw Authorization header value with no scheme prefix\n    — Authorization: <api-key>'\n  issued_at: the API Keys tab of the Immuta user profile page\n- name: immutaBearerExchange\n  type: http\n  scheme: bearer\n  surface: Immuta Govern API\n  sources: [https://documentation.immuta.com/saas/developer-guides/api-intro/authentication]\n  exchange:\n    endpoint: POST /bim/apikey/authenticate\n    request: '{\"apikey\": \"<your-api-key>\"}'\n    response: bearer\
  \ token presented as Authorization Bearer on subsequent calls\nauthorization_model:\n  mechanism: Immuta permissions and roles on the calling identity\n  examples: [CREATE_DATA_SOURCE, APPLICATION_ADMIN]\n  scopes: []\n  note: 'documented per endpoint as \"Required Immuta permission\"; scopes/ is intentionally\n    not emitted for this provider because there is no OAuth scope surface to record.'\ngaps:\n- The published OpenAPI applies no security requirement at the document level and none\n  at the operation level, so the declared bearer scheme is never bound to an operation\n  in the contract (see overlays/immuta-marketplace-api-overlay.yaml).\n- No 401 or 403 response is declared on any operation.\n- No token refresh, rotation or revocation policy is published for Govern API keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immuta/refs/heads/main/authentication/immuta-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Data Governance
- Data Access Control
- Data Security
- Data Privacy
- Policy Management
- Data Marketplace
- Compliance
- Snowflake
- Databricks
- Analytics
- Agentic Data Access
---
