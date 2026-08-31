---
api_key_in: []
api_specs:
- filename: turquoise-health-consumer-pricing-api-openapi.yml
  format: yaml
  label: Turquoise Health Consumer Pricing API
  slug: turquoise-health-consumer-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/openapi/turquoise-health-consumer-pricing-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Turquoise Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Turquoise Health secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Turquoise Health
provider_slug: turquoise-health
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/turquoise-health-consumer-pricing-openapi.yml
  type: http
- description: OAuth2 access token issued by Turquoise; validated against turquoise-api's /oauth/authorize on every request.
  name: PartnerBearerToken
  scheme: bearer
  sources:
  - openapi/turquoise-health-consumer-pricing-openapi.yml
  type: http
slug: turquoise-health-authentication
source_filename: turquoise-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/turquoise-health-consumer-pricing-openapi.yml\ndocs: https://turquoise.health/api/docs/start-building/\ndocs_markdown: https://turquoise.health/api/docs/start-building.md\nnote: >-\n  Upgraded from the derived baseline. The OpenAPI declares two http/bearer schemes but no\n  oauth2 securityScheme and no global security[] requirement, so the spec alone understates\n  the real model. The published Start Building guide documents the actual contract: a\n  single OAuth 2.0 client-credentials flow whose token authenticates BOTH the REST API and\n  the MCP server. The MCP host additionally serves RFC 8414 + RFC 9728 metadata anonymously.\n\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  shared_token: >-\n    The same access token authenticates the Consumer Pricing REST API\n    (https://api.turquoise.health) and the MCP server\n   \
  \ (https://consumer-mcp.turquoise.health/mcp).\n\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources: [openapi/turquoise-health-consumer-pricing-openapi.yml]\n- name: PartnerBearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    OAuth2 access token issued by Turquoise; validated against turquoise-api's\n    /oauth/authorize on every request.\n  sources: [openapi/turquoise-health-consumer-pricing-openapi.yml]\n\noauth2:\n  flow: client_credentials\n  token_endpoint: https://api.turquoise.health/oauth/token\n  token_request:\n    method: POST\n    content_type: application/json\n    parameters: [grant_type, client_id, client_secret, organization_id]\n    note: >-\n      Credentials are a client_id, client_secret and organization_id. Unusually, the token\n      request body is JSON rather than form-encoded, and organization_id is a required\n      third credential alongside the usual client pair.\n  token_response:\n    access_token:\
  \ Bearer token to send on every request.\n    token_type: Always \"Bearer\".\n    expires_in: Seconds until expiry (documented example 3600).\n  expiry_note: >-\n    The docs state expires_in in the example is 3600 (one hour) but also advise that\n    \"access tokens are valid for a week\" and recommend caching rather than minting per\n    request. Treat expires_in on the live response as authoritative and refresh\n    proactively rather than waiting for a 401.\n  on_expiry: Requests receive HTTP 401 Unauthorized; repeat the token request to obtain a new one.\n\nrequest_header:\n  name: Authorization\n  format: 'Bearer <token>'\n  applies_to:\n  - https://api.turquoise.health (every v3 request)\n  - https://consumer-mcp.turquoise.health/mcp (every MCP request)\n\ninteractive_alternative:\n  applies_to: MCP only\n  description: >-\n    MCP-capable interactive clients (Claude Code, Claude Desktop, Codex, Cursor) sign in\n    through the browser with a Turquoise account, so there is no token\
  \ to manage; the\n    server then scopes calls to that user's organization.\n\ndiscovery:\n  authorization_server_metadata:\n    url: https://consumer-mcp.turquoise.health/.well-known/oauth-authorization-server\n    spec: RFC 8414\n    status: 200\n    file: well-known/turquoise-health-oauth-authorization-server.json\n  protected_resource_metadata:\n    url: https://consumer-mcp.turquoise.health/.well-known/oauth-protected-resource/mcp\n    spec: RFC 9728\n    status: 200\n    file: well-known/turquoise-health-oauth-protected-resource.json\n\ncredential_acquisition:\n  test: https://turquoise.health/signup/?signupContext=api\n  test_note: Free sign-up returns test credentials in a demo account.\n  production: https://turquoise.health/request-a-demo\n  production_note: >-\n    Production access is required to send real PHI to the personalized-estimates endpoint\n    and mandates a signed Business Associate Agreement (BAA) with Turquoise.\n\nauth_errors:\n- status: 401\n  meaning: Missing,\
  \ expired, or wrong-audience token.\n- status: 403\n  meaning: Token is valid but not granted the correct scope.\n- code: unauthorized\n  surface: personalized-estimates\n- code: forbidden\n  surface: personalized-estimates\n- code: insufficient_scope\n  surface: v3\n- code: authorization_unavailable\n  surface: personalized-estimates\n\nsee_also:\n- scopes/turquoise-health-scopes.yml\n- conventions/turquoise-health-conventions.yml\n- well-known/turquoise-health-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/authentication/turquoise-health-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- Price Transparency
- Hospital Rates
- Payer Rates
- Machine-Readable Files
- FHIR
- Health Insurance
- Negotiated Rates
- Out-of-Pocket Costs
- MRF
- Consumer Pricing
- MCP
- Eligibility
- Standard Service Packages
- HIPAA
---
