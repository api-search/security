---
api_key_in: []
api_specs:
- filename: cb-insights-authorization-api-openapi.yml
  format: yaml
  label: CB Insights Authorization API
  slug: cb-insights-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-authorization-api-openapi.yml
- filename: cb-insights-businessrelationships-api-openapi.yml
  format: yaml
  label: CB Insights Business Relationships API
  slug: cb-insights-businessrelationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-businessrelationships-api-openapi.yml
- filename: cb-insights-chatcbi-api-openapi.yml
  format: yaml
  label: CB Insights Chat CBI API
  slug: cb-insights-chatcbi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-chatcbi-api-openapi.yml
- filename: cb-insights-financialtransactions-api-openapi.yml
  format: yaml
  label: CB Insights Financial Transactions API
  slug: cb-insights-financialtransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-financialtransactions-api-openapi.yml
- filename: cb-insights-firmographics-api-openapi.yml
  format: yaml
  label: CB Insights Firmographics API
  slug: cb-insights-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-firmographics-api-openapi.yml
- filename: cb-insights-managementandboard-api-openapi.yml
  format: yaml
  label: CB Insights Management And Board API
  slug: cb-insights-managementandboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-managementandboard-api-openapi.yml
- filename: cb-insights-organizations-api-openapi.yml
  format: yaml
  label: CB Insights Organizations API
  slug: cb-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-organizations-api-openapi.yml
- filename: cb-insights-outlook-api-openapi.yml
  format: yaml
  label: CB Insights Outlook API
  slug: cb-insights-outlook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-outlook-api-openapi.yml
- filename: cb-insights-revenue-api-openapi.yml
  format: yaml
  label: CB Insights Revenue API
  slug: cb-insights-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-revenue-api-openapi.yml
- filename: cb-insights-scoutingreports-api-openapi.yml
  format: yaml
  label: CB Insights Scouting Reports API
  slug: cb-insights-scoutingreports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-scoutingreports-api-openapi.yml
- filename: cb-insights-strategymap-api-openapi.yml
  format: yaml
  label: CB Insights Strategy Map API
  slug: cb-insights-strategymap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-strategymap-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cb Insights Authentication
name_suffix: Authentication
oauth_flows: []
overview: CB Insights declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: CB Insights
provider_slug: cb-insights
scheme_count: 4
schemes:
- applies_to: CB Insights API v2 (all 28 operations except POST /v2/authorize)
  description: Bearer JWT required on every v2 data operation. Declared in the published Swagger 2.0 contract as an apiKey-in-header scheme (Swagger 2.0 has no bearer http type), and additionally declared as a required `Authorization` header parameter on each operation.
  format: Bearer <JWT>
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/_original/cb-insights-api-v2-openapi.json
  - https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication
  type: apiKey
- method: POST
  name: v2 client credentials exchange
  notes: Documented as a "client credentials flow" but it is NOT RFC 6749 — the request is a bespoke JSON body against /v2/authorize rather than an OAuth token endpoint with grant_type. The quick-start shows an `expiresIn` field alongside `token`; the authentication reference states the token is valid 24 hours and that there is no refresh-token mechanism (re-authorize on expiry).
  request_body: '{"clientId": "...", "clientSecret": "..."}'
  response_body: '{"token": "..."}'
  sources:
  - https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication
  - https://api-docs.cbinsights.com/portal/docs/quick-start
  token_endpoint: https://api.cbinsights.com/v2/authorize
  type: custom-client-credentials
- method: GET
  name: v1 JWT authorize
  notes: The v1 flow passes the client secret as a URL query parameter on a GET request, which puts the long-lived secret into proxy, browser and server access logs. v2 moved this to a POST body.
  request: query parameters clientId + clientSecret
  response_body: '{"token": "..."}'
  sources:
  - https://api-docs.cbinsights.com/docs/tutorials/authentication_flow/
  - https://api-docs.cbinsights.com/docs/endpoints/authentication_endpoint/
  token_endpoint: https://api.cbinsights.com/v1/authorize
  token_lifetime: 24h
  type: custom-client-credentials
- applies_to: CB Insights MCP Server (https://mcp.cbinsights.com/)
  authorization_endpoint: https://mcp.cbinsights.com/authorize
  bearer_methods_supported:
  - header
  discovery:
    oauth_authorization_server: well-known/cb-insights-mcp-oauth-authorization-server.json
    oauth_protected_resource: well-known/cb-insights-mcp-oauth-protected-resource.json
    openid_configuration: well-known/cb-insights-mcp-openid-configuration.json
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  issuer: https://mcp.cbinsights.com/
  name: MCP OAuth 2.1
  notes: Dynamic client registration is open (registration_endpoint present, token_endpoint_auth_methods includes "none"), which is what makes one-click connector setup work in Claude/ChatGPT/Copilot. The three scopes advertised are identity scopes only — no data-permission scopes are published, so authorization granularity is not expressed in the token.
  pkce:
  - S256
  registration_endpoint: https://mcp.cbinsights.com/register
  response_types:
  - code
  scopes_supported:
  - openid
  - email
  - profile
  sources:
  - https://mcp.cbinsights.com/.well-known/oauth-authorization-server
  - https://mcp.cbinsights.com/.well-known/oauth-protected-resource
  token_endpoint: https://mcp.cbinsights.com/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: cb-insights-authentication
source_filename: cb-insights-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication\ndocs:\n- https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication\n- https://api-docs.cbinsights.com/portal/docs/quick-start\n- https://api-docs.cbinsights.com/docs/tutorials/authentication_flow/\n- https://api-docs.cbinsights.com/docs/endpoints/authentication_endpoint/\nderived_from:\n- openapi/_original/cb-insights-api-v2-openapi.json\n- well-known/cb-insights-mcp-oauth-authorization-server.json\n- well-known/cb-insights-mcp-oauth-protected-resource.json\nsummary: >-\n  Three distinct authentication models across the CB Insights estate. The REST APIs (v1 and v2) both\n  use a CB-Insights-issued clientId/clientSecret pair exchanged at an /authorize endpoint for a\n  bearer JWT, which is then sent in the Authorization header of every data call; there is no refresh\n  token. The hosted MCP server is separate — it is a full OAuth 2.1 authorization\
  \ server with\n  dynamic client registration and PKCE, which is what lets Claude/ChatGPT/Copilot connect with an\n  end-user login rather than an API credential. Credentials are never self-issued: clientId and\n  clientSecret come from a CB Insights representative or from the developer-portal trial sign-up.\ntypes:\n- apiKey\n- oauth2\napi_key_in:\n- header\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Bearer <JWT>\n  description: >-\n    Bearer JWT required on every v2 data operation. Declared in the published Swagger 2.0 contract as\n    an apiKey-in-header scheme (Swagger 2.0 has no bearer http type), and additionally declared as a\n    required `Authorization` header parameter on each operation.\n  applies_to: CB Insights API v2 (all 28 operations except POST /v2/authorize)\n  sources:\n  - openapi/_original/cb-insights-api-v2-openapi.json\n  - https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication\n- name: v2 client\
  \ credentials exchange\n  type: custom-client-credentials\n  token_endpoint: https://api.cbinsights.com/v2/authorize\n  method: POST\n  request_body: '{\"clientId\": \"...\", \"clientSecret\": \"...\"}'\n  response_body: '{\"token\": \"...\"}'\n  notes: >-\n    Documented as a \"client credentials flow\" but it is NOT RFC 6749 — the request is a bespoke JSON\n    body against /v2/authorize rather than an OAuth token endpoint with grant_type. The quick-start\n    shows an `expiresIn` field alongside `token`; the authentication reference states the token is\n    valid 24 hours and that there is no refresh-token mechanism (re-authorize on expiry).\n  sources:\n  - https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication\n  - https://api-docs.cbinsights.com/portal/docs/quick-start\n- name: v1 JWT authorize\n  type: custom-client-credentials\n  token_endpoint: https://api.cbinsights.com/v1/authorize\n  method: GET\n  request: query parameters clientId + clientSecret\n  response_body:\
  \ '{\"token\": \"...\"}'\n  token_lifetime: 24h\n  notes: >-\n    The v1 flow passes the client secret as a URL query parameter on a GET request, which puts the\n    long-lived secret into proxy, browser and server access logs. v2 moved this to a POST body.\n  sources:\n  - https://api-docs.cbinsights.com/docs/tutorials/authentication_flow/\n  - https://api-docs.cbinsights.com/docs/endpoints/authentication_endpoint/\n- name: MCP OAuth 2.1\n  type: oauth2\n  applies_to: CB Insights MCP Server (https://mcp.cbinsights.com/)\n  issuer: https://mcp.cbinsights.com/\n  authorization_endpoint: https://mcp.cbinsights.com/authorize\n  token_endpoint: https://mcp.cbinsights.com/token\n  registration_endpoint: https://mcp.cbinsights.com/register\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  response_types:\n  - code\n  pkce:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  scopes_supported:\n  - openid\n\
  \  - email\n  - profile\n  bearer_methods_supported:\n  - header\n  discovery:\n    oauth_authorization_server: well-known/cb-insights-mcp-oauth-authorization-server.json\n    oauth_protected_resource: well-known/cb-insights-mcp-oauth-protected-resource.json\n    openid_configuration: well-known/cb-insights-mcp-openid-configuration.json\n  notes: >-\n    Dynamic client registration is open (registration_endpoint present, token_endpoint_auth_methods\n    includes \"none\"), which is what makes one-click connector setup work in Claude/ChatGPT/Copilot.\n    The three scopes advertised are identity scopes only — no data-permission scopes are published,\n    so authorization granularity is not expressed in the token.\n  sources:\n  - https://mcp.cbinsights.com/.well-known/oauth-authorization-server\n  - https://mcp.cbinsights.com/.well-known/oauth-protected-resource\ncredential_issuance:\n  self_serve: partial\n  detail: >-\n    A trial clientId/clientSecret is issued through the developer-portal\
  \ sign-up form after email\n    validation (25 companies, 5 scouting reports, 5 ChatCBI messages). Production credentials are\n    issued by a CB Insights representative / CSM — there is no self-serve production key.\n  sign_up: https://api-docs.cbinsights.com/portal/signup\nenterprise_identity:\n  saml_sso:\n    supported: true\n    initiation: SP-initiated only (IdP-initiated SSO is explicitly not supported)\n    idps_documented:\n    - Okta (Okta Integration Network app)\n    - Azure AD\n    docs: https://docs.cbinsights.com/docs/sso/index.html\n  scim:\n    supported: true\n    version_documented: SCIM (version not stated)\n    operations:\n    - create users\n    - update user attributes\n    - deactivate users\n    primary_identifier: email mapped to SCIM userName\n    credential: SCIM API key generated in Account Settings > Single Sign-On\n    docs: https://docs.cbinsights.com/docs/scim/index.html\n  mfa:\n    supported: true\n    source: https://www.cbinsights.com/security-and-privacy/\n\
  gaps:\n- No RFC 6749 / RFC 8414 conformance on the REST token endpoint — the \"client credentials flow\" is a\n  bespoke JSON exchange, so standard OAuth clients cannot be pointed at it.\n- No refresh token on the REST APIs; every 24 hours the client must resend the long-lived secret.\n- v1 transmits clientSecret in a URL query string.\n- No token revocation, introspection, or key-rotation endpoint is documented.\n- The MCP authorization server advertises only openid/email/profile — no data scopes, so an agent\n  token cannot be narrowed to a subset of the data surface.\ncross_links:\n  conformance: conformance/cb-insights-conformance.yml\n  conventions: conventions/cb-insights-conventions.yml\n  well_known: well-known/cb-insights-well-known.yml\n  mcp: mcp/cb-insights-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/authentication/cb-insights-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Market Intelligence
- private-company-data
- venture-capital
- funding-data
- investor-data
- company-data
- people-data
- business-relationships
- predictive-scoring
- MCP
- agent-native
- Data Enrichment
- snowflake
---
