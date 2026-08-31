---
api_key_in: []
api_specs:
- filename: criteo-accounts-api-openapi.yml
  format: yaml
  label: Criteo Accounts API
  slug: criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-accounts-api-openapi.yml
- filename: criteo-advertiser-api-openapi.yml
  format: yaml
  label: Criteo Advertiser API
  slug: criteo-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-advertiser-api-openapi.yml
- filename: criteo-analytics-api-openapi.yml
  format: yaml
  label: Criteo Analytics API
  slug: criteo-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-analytics-api-openapi.yml
- filename: criteo-audience-api-openapi.yml
  format: yaml
  label: Criteo Audience API
  slug: criteo-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-audience-api-openapi.yml
- filename: criteo-balance-api-openapi.yml
  format: yaml
  label: Criteo Balance API
  slug: criteo-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-balance-api-openapi.yml
- filename: criteo-billing-api-openapi.yml
  format: yaml
  label: Criteo Billing API
  slug: criteo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-billing-api-openapi.yml
- filename: criteo-campaign-api-openapi.yml
  format: yaml
  label: Criteo Campaign API
  slug: criteo-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-campaign-api-openapi.yml
- filename: criteo-catalog-api-openapi.yml
  format: yaml
  label: Criteo Catalog API
  slug: criteo-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-catalog-api-openapi.yml
- filename: criteo-creative-api-openapi.yml
  format: yaml
  label: Criteo Creative API
  slug: criteo-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-creative-api-openapi.yml
- filename: criteo-gateway-api-openapi.yml
  format: yaml
  label: Criteo Gateway API
  slug: criteo-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-gateway-api-openapi.yml
- filename: criteo-reco-api-openapi.yml
  format: yaml
  label: Criteo Reco API
  slug: criteo-reco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-reco-api-openapi.yml
- filename: criteo-segment-api-openapi.yml
  format: yaml
  label: Criteo Segment API
  slug: criteo-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-segment-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Criteo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Criteo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Criteo
provider_slug: criteo
scheme_count: 1
schemes:
- flows:
  - declared_scopes: 0
    flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    declared_scopes: 0
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  note: The flow `scopes` maps are empty in all three specs; the 22 real scope strings live on per-operation security requirements. See scopes/criteo-scopes.yml.
  sources:
  - openapi/criteo-retail-media-api-openapi.yml
  - openapi/criteo-marketing-solutions-api-openapi.yml
  - openapi/criteo-commerce-grid-api-openapi.yml
  type: oauth2
slug: criteo-authentication
source_filename: criteo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/criteo-retail-media-api-openapi.yml, openapi/criteo-marketing-solutions-api-openapi.yml, openapi/criteo-commerce-grid-api-openapi.yml\ndocs: https://developers.criteo.com/criteo-apis/docs/api-authorization\nsupersedes: >-\n  Rewritten 2026-08-13 against Criteo's real published OpenAPI. The prior version was derived\n  from a hand-authored scaffold and carried an authorizationUrl of\n  https://consent.criteo.com/authorize; the real spec and the real RFC 8414 metadata both\n  give different values, recorded below.\n\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  api_key_in: []\n  scope_count: 22\n  token_transport: Bearer token in the Authorization header\n  token_lifetime_seconds: 900\n  anonymous_operations: 0\n  security_coverage: >-\n    All 219 operations across the three specs declare a security requirement — there are no\n    unauthenticated operations. Four of them require\
  \ a valid token but no specific scope\n    (empty scope array): GetCurrentApplication in each of the three services, and\n    ListAdvertisers in Marketing Solutions.\n  token_endpoint_not_in_spec: >-\n    POST https://api.criteo.com/oauth2/token is NOT declared in any of the three published\n    OpenAPI documents. The one operation every client must call first is absent from the\n    machine-readable contract and exists only in prose. An agent bootstrapping purely from\n    the spec cannot obtain a token.\n\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n    declared_scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n    declared_scopes: 0\n  sources:\n  - openapi/criteo-retail-media-api-openapi.yml\n  - openapi/criteo-marketing-solutions-api-openapi.yml\n  - openapi/criteo-commerce-grid-api-openapi.yml\n  note:\
  \ >-\n    The flow `scopes` maps are empty in all three specs; the 22 real scope strings live on\n    per-operation security requirements. See scopes/criteo-scopes.yml.\n\ngrants:\n- grant: client_credentials\n  audience: Server-to-server integrations acting for the app owner\n  rate_limit: 250 calls/min default, 40 calls/min on reporting endpoints\n  rate_limit_applies_at: application level\n  consent_required: false\n  note: >-\n    A single shared access token per application. Criteo's own rate-limit guidance warns that\n    this is the constraining choice for multi-tenant platforms: ten concurrent users share\n    one 250/min budget.\n- grant: authorization_code\n  audience: Self-service platforms acting on behalf of a consenting advertiser\n  rate_limit: 10 calls/min per consented account, scaling linearly with accounts consented\n  rate_limit_applies_at: account level\n  consent_required: true\n  consent_url: https://consent.criteo.com/request\n  revocable: true\n  revocation_note:\
  \ >-\n    Advertisers manage and revoke app access from a consent dashboard. A revoked grant\n    surfaces as HTTP 403 on subsequent calls, not 401.\n- grant: refresh_token\n  audience: Authorization Code applications refreshing an expired access token\n  source: https://mcp.criteo.com/.well-known/oauth-authorization-server\n\ndiscovery:\n  rfc8414_metadata: https://mcp.criteo.com/.well-known/oauth-authorization-server\n  rfc9728_metadata: https://mcp.criteo.com/.well-known/oauth-protected-resource\n  issuer: https://api.criteo.com\n  authorization_endpoint: https://consent.criteo.com/request\n  token_endpoint: https://api.criteo.com/oauth2/token\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  bearer_methods_supported: [header]\n  saved_to: [well-known/criteo-oauth-authorization-server.json, well-known/criteo-oauth-protected-resource.json]\n  finding: >-\n    Criteo publishes RFC 8414 authorization-server metadata, but ONLY on the MCP\
  \ host\n    (mcp.criteo.com). The same path returns 404 on api.criteo.com and developers.criteo.com,\n    so a client that discovers Criteo through the REST API or the docs cannot find it. The\n    metadata it publishes also omits client_credentials from grant_types_supported even\n    though the REST API's primary grant IS client_credentials — the document describes the\n    MCP server's grants, not the platform's.\n\napplication_model:\n  docs: https://developers.criteo.com/criteo-apis/docs/create-your-app\n  credentials_docs: https://developers.criteo.com/criteo-apis/docs/get-credentials\n  steps:\n  - Create a partner account on the developer portal\n  - Create an organization\n  - Create an API application, choosing a service and a per-domain authorization level\n  - Retrieve client_id and client_secret\n  - For Authorization Code apps, generate a consent URL and have the advertiser grant access\n  note: >-\n    Credentials are issued per application, not per user, and the permission\
  \ set is fixed at\n    app-configuration time rather than requested per token.\n\nerrors:\n  '401': Missing, malformed or expired token\n  '403': >-\n    Valid token, but the application lacks permission on the advertiser or domain, or consent\n    was never granted or has been revoked. Criteo's guidance is to relaunch the OAuth2 flow.\n  caveat: >-\n    On BULK endpoints a missing resource or an insufficient permission returns HTTP 200 with\n    an empty response rather than 403 — documented by Criteo and important for any agent that\n    treats 200 as success.\n  reference: https://developers.criteo.com/criteo-apis/docs/api-error-codes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/authentication/criteo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Agent Skills
- Analytics
- Audiences
- Campaigns
- Catalog
- Commerce
- Commerce Media
- Display Advertising
- Marketing
- MCP
- Media
- Authentication
- OpenAPI
- Reporting
- Retail
- Retail Media
- Sponsored Products
---
