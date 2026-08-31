---
api_key_in: []
api_specs:
- filename: daloopa-auth-api-openapi.yml
  format: yaml
  label: Daloopa Auth API
  slug: daloopa-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-auth-api-openapi.yml
- filename: daloopa-companies-api-openapi.yml
  format: yaml
  label: Daloopa Companies API
  slug: daloopa-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-companies-api-openapi.yml
- filename: daloopa-consumption-api-openapi.yml
  format: yaml
  label: Daloopa Consumption API
  slug: daloopa-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-consumption-api-openapi.yml
- filename: daloopa-daloopa-mcp-service-api-openapi.yml
  format: yaml
  label: Daloopa Daloopa MCP Service API
  slug: daloopa-daloopa-mcp-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-daloopa-mcp-service-api-openapi.yml
- filename: daloopa-data-warehouse-api-openapi.yml
  format: yaml
  label: Daloopa Data Warehouse API
  slug: daloopa-data-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-data-warehouse-api-openapi.yml
- filename: daloopa-databricks-api-openapi.yml
  format: yaml
  label: Daloopa Databricks API
  slug: daloopa-databricks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-databricks-api-openapi.yml
- filename: daloopa-documents-api-openapi.yml
  format: yaml
  label: Daloopa Documents API
  slug: daloopa-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-documents-api-openapi.yml
- filename: daloopa-download-api-openapi.yml
  format: yaml
  label: Daloopa Download API
  slug: daloopa-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-download-api-openapi.yml
- filename: daloopa-export-api-openapi.yml
  format: yaml
  label: Daloopa Export API
  slug: daloopa-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-export-api-openapi.yml
- filename: daloopa-fundamentals-api-openapi.yml
  format: yaml
  label: Daloopa Fundamentals API
  slug: daloopa-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-fundamentals-api-openapi.yml
- filename: daloopa-health-api-openapi.yml
  format: yaml
  label: Daloopa Health API
  slug: daloopa-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-health-api-openapi.yml
- filename: daloopa-industry-models-api-openapi.yml
  format: yaml
  label: Daloopa Industry Models API
  slug: daloopa-industry-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-industry-models-api-openapi.yml
- filename: daloopa-investing-skills-api-openapi.yml
  format: yaml
  label: Daloopa Investing Skills API
  slug: daloopa-investing-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-investing-skills-api-openapi.yml
- filename: daloopa-market-data-api-openapi.yml
  format: yaml
  label: Daloopa Market Data API
  slug: daloopa-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-market-data-api-openapi.yml
- filename: daloopa-partnership-api-openapi.yml
  format: yaml
  label: Daloopa Partnership API
  slug: daloopa-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-partnership-api-openapi.yml
- filename: daloopa-series-api-openapi.yml
  format: yaml
  label: Daloopa Series API
  slug: daloopa-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-series-api-openapi.yml
- filename: daloopa-snowflake-api-openapi.yml
  format: yaml
  label: Daloopa Snowflake API
  slug: daloopa-snowflake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-snowflake-api-openapi.yml
- filename: daloopa-taxonomy-api-openapi.yml
  format: yaml
  label: Daloopa Taxonomy API
  slug: daloopa-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-taxonomy-api-openapi.yml
- filename: daloopa-webhooks-api-openapi.yml
  format: yaml
  label: Daloopa Webhooks API
  slug: daloopa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Daloopa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daloopa secures its APIs with http, oauth2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Daloopa
provider_slug: daloopa
scheme_count: 4
schemes:
- applies_to: https://app.daloopa.com/api/v3
  credential_format: base64(<email>:<api_key>)
  description: 'Basic authentication with base64-encoded credentials. Format: "Basic base64(email:apiKey)"'
  example_form: 'Authorization: Basic base64(email:api_key)'
  header: Authorization
  name: apiKeyAuth
  scheme: basic
  sources:
  - openapi/daloopa-api-openapi.yml
  - https://docs.daloopa.com/docs/api-authentication
  surface: rest
  type: http
- applies_to: https://mcp.daloopa.com/server/mcp
  authorization_endpoint: https://mcp.daloopa.com/authorize
  description: MCP OAuth per the Model Context Protocol authorization specification. Anonymous discovery is served from the MCP host; an unauthenticated tools/list returns 401 with a WWW-Authenticate Bearer challenge naming the protected-resource metadata document.
  discovery:
    authorization_server: well-known/daloopa-mcp-oauth-authorization-server.json
    protected_resource: well-known/daloopa-mcp-oauth-protected-resource.json
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  issuer: https://mcp.daloopa.com
  name: mcpOAuth
  pkce: S256
  registration_endpoint: https://mcp.daloopa.com/register
  response_types:
  - code
  scopes_note: The authorization-server metadata document does NOT advertise a scopes_supported array, and no scope reference is published in the docs. No OAuthScopes artifact is emitted because there are no published scopes to record — an honest absence, not an unchecked field.
  scopes_supported: null
  sources:
  - https://docs.daloopa.com/docs/mcp-authentication
  - https://mcp.daloopa.com/.well-known/oauth-authorization-server
  - https://mcp.daloopa.com/.well-known/oauth-protected-resource
  surface: mcp
  token_endpoint: https://mcp.daloopa.com/token
  token_endpoint_auth_methods:
  - client_secret_post
  type: oauth2
- description: API-key-for-token exchange. POST an existing Daloopa API key to the token endpoint to mint a bearer token without running the OAuth flow. Tokens are valid for 24 hours, after which a new token must be requested.
  name: mcpBearerToken
  operation: api_key_token_auth_token_post
  scheme: bearer
  sources:
  - https://docs.daloopa.com/docs/mcp-authentication
  - openapi/daloopa-mcp-service-openapi.json
  surface: mcp
  token_exchange_endpoint: https://mcp.daloopa.com/auth/token
  token_lifetime: 24h
  type: http
- description: Direct header-based API key authentication for callers who prefer not to mint or refresh a token. The API key is sent with every request; no token generation or refresh is required.
  header: X-API-KEY
  in: header
  name: mcpApiKeyHeader
  sources:
  - https://docs.daloopa.com/docs/mcp-authentication
  surface: mcp
  type: apiKey
slug: daloopa-authentication
source_filename: daloopa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://docs.daloopa.com/docs/api-authentication\ndocs: https://docs.daloopa.com/docs/api-authentication\nmcp_docs: https://docs.daloopa.com/docs/mcp-authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  - apiKey\n  note: >-\n    Two independent surfaces with different auth. The REST API v3 accepts ONLY HTTP Basic carrying\n    base64(email:api_key). The hosted MCP server accepts three methods: MCP OAuth 2.1 (dynamic client\n    registration + PKCE S256), a 24-hour bearer token minted from an API key, or a direct X-API-KEY header.\n\nschemes:\n- name: apiKeyAuth\n  surface: rest\n  type: http\n  scheme: basic\n  description: 'Basic authentication with base64-encoded credentials. Format: \"Basic base64(email:apiKey)\"'\n  header: Authorization\n  credential_format: base64(<email>:<api_key>)\n  example_form: 'Authorization: Basic base64(email:api_key)'\n  applies_to: https://app.daloopa.com/api/v3\n  sources:\n  - openapi/daloopa-api-openapi.yml\n\
  \  - https://docs.daloopa.com/docs/api-authentication\n\n- name: mcpOAuth\n  surface: mcp\n  type: oauth2\n  description: >-\n    MCP OAuth per the Model Context Protocol authorization specification. Anonymous discovery is served\n    from the MCP host; an unauthenticated tools/list returns 401 with a WWW-Authenticate Bearer challenge\n    naming the protected-resource metadata document.\n  applies_to: https://mcp.daloopa.com/server/mcp\n  issuer: https://mcp.daloopa.com\n  authorization_endpoint: https://mcp.daloopa.com/authorize\n  token_endpoint: https://mcp.daloopa.com/token\n  registration_endpoint: https://mcp.daloopa.com/register\n  grant_types: [authorization_code]\n  response_types: [code]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_post]\n  dynamic_client_registration: true\n  scopes_supported: null\n  scopes_note: >-\n    The authorization-server metadata document does NOT advertise a scopes_supported array, and no scope\n    reference is published in the docs.\
  \ No OAuthScopes artifact is emitted because there are no published\n    scopes to record — an honest absence, not an unchecked field.\n  discovery:\n    authorization_server: well-known/daloopa-mcp-oauth-authorization-server.json\n    protected_resource: well-known/daloopa-mcp-oauth-protected-resource.json\n  sources:\n  - https://docs.daloopa.com/docs/mcp-authentication\n  - https://mcp.daloopa.com/.well-known/oauth-authorization-server\n  - https://mcp.daloopa.com/.well-known/oauth-protected-resource\n\n- name: mcpBearerToken\n  surface: mcp\n  type: http\n  scheme: bearer\n  description: >-\n    API-key-for-token exchange. POST an existing Daloopa API key to the token endpoint to mint a bearer\n    token without running the OAuth flow. Tokens are valid for 24 hours, after which a new token must be requested.\n  token_exchange_endpoint: https://mcp.daloopa.com/auth/token\n  token_lifetime: 24h\n  operation: api_key_token_auth_token_post\n  sources:\n  - https://docs.daloopa.com/docs/mcp-authentication\n\
  \  - openapi/daloopa-mcp-service-openapi.json\n\n- name: mcpApiKeyHeader\n  surface: mcp\n  type: apiKey\n  in: header\n  header: X-API-KEY\n  description: >-\n    Direct header-based API key authentication for callers who prefer not to mint or refresh a token.\n    The API key is sent with every request; no token generation or refresh is required.\n  sources:\n  - https://docs.daloopa.com/docs/mcp-authentication\n\nkey_management:\n  rotation: >-\n    \"API keys will be rotated on a six-month cycle to ensure ongoing security\" — published policy on the\n    authentication page.\n  rotation_period: 6 months\n  ip_allowlisting:\n    available: true\n    note: IP validation can be enabled on request to restrict API access to pre-approved addresses.\n  sso:\n    available: true\n    protocol: SAML/OIDC via Microsoft Entra (Azure AD)\n    docs: https://docs.daloopa.com/docs/single-sign-on\n    note: Applies to the Daloopa application account, not to API credentials directly.\n\nobservations:\n\
  - >-\n  The REST API v3 deliberately RETIRED the legacy plaintext-API-key scheme; v3 accepts only the encoded\n  email+key Basic form. v2 still accepts both during the migration window. This is a genuine auth\n  hardening, versioned rather than shipped silently.\n- >-\n  The two surfaces do not share an auth mechanism. An agent that holds a working REST credential cannot\n  call the MCP server with it as-is without either the token exchange or the X-API-KEY header form.\n\ncross_links:\n  conventions: conventions/daloopa-conventions.yml\n  conformance: conformance/daloopa-conformance.yml\n  well_known: well-known/daloopa-well-known.yml\n  lifecycle: lifecycle/daloopa-lifecycle.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/authentication/daloopa-authentication.yml
summary_line: http/oauth2/apiKey · 4 schemes
tags:
- Financial Data
- Fundamental Data
- Market Data
- Investment Research
- Equity Research
- SEC Filings
- Earnings
- Fintech
- MCP
- agent-native
- Agent Skills
- Webhook
- Data Warehouse
---
