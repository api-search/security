---
api_key_in: []
api_specs:
- filename: scope3-buyer-openapi-original.yml
  format: yaml
  label: Scope3 Interchange Buyer API
  slug: scope3-interchange-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/_original/scope3-buyer-openapi-original.yml
- filename: scope3-storefront-openapi-original.yml
  format: yaml
  label: Scope3 Interchange Storefront API
  slug: scope3-interchange-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/_original/scope3-storefront-openapi-original.yml
- filename: scope3-ai-impact-measurement-api-openapi.yml
  format: yaml
  label: Scope3 AI Impact Measurement API
  slug: scope3-ai-impact-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-ai-impact-measurement-api-openapi.yml
- filename: scope3-benchmarks-api-openapi.yml
  format: yaml
  label: Scope3 Benchmarks API
  slug: scope3-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-benchmarks-api-openapi.yml
- filename: scope3-creative-api-openapi.yml
  format: yaml
  label: Scope3 Creative API
  slug: scope3-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-creative-api-openapi.yml
- filename: scope3-data-api-openapi.yml
  format: yaml
  label: Scope3 Data API
  slug: scope3-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-data-api-openapi.yml
- filename: scope3-gpu-api-openapi.yml
  format: yaml
  label: Scope3 Gpu API
  slug: scope3-gpu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-gpu-api-openapi.yml
- filename: scope3-impact-api-openapi.yml
  format: yaml
  label: Scope3 Impact API
  slug: scope3-impact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-impact-api-openapi.yml
- filename: scope3-measure-api-openapi.yml
  format: yaml
  label: Scope3 Measure API
  slug: scope3-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-measure-api-openapi.yml
- filename: scope3-model-api-openapi.yml
  format: yaml
  label: Scope3 Model API
  slug: scope3-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-model-api-openapi.yml
- filename: scope3-node-api-openapi.yml
  format: yaml
  label: Scope3 Node API
  slug: scope3-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-node-api-openapi.yml
- filename: scope3-reload-api-openapi.yml
  format: yaml
  label: Scope3 Reload API
  slug: scope3-reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-reload-api-openapi.yml
- filename: scope3-saved-lists-api-openapi.yml
  format: yaml
  label: Scope3 Saved Lists API
  slug: scope3-saved-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-saved-lists-api-openapi.yml
- filename: scope3-segment-api-openapi.yml
  format: yaml
  label: Scope3 Segment API
  slug: scope3-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-segment-api-openapi.yml
- filename: scope3-signals-api-openapi.yml
  format: yaml
  label: Scope3 Signals API
  slug: scope3-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-signals-api-openapi.yml
- filename: scope3-status-api-openapi.yml
  format: yaml
  label: Scope3 Status API
  slug: scope3-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-status-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Scope3 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: Scope3 secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: Scope3
provider_slug: scope3
scheme_count: 4
schemes:
- applies_to: Carbon Calculator (api.scope3.com/v2), AI Impact Measurement (aiapi.scope3.com)
  bearerFormat: JWT
  docs: https://docs.scope3.com/docs/access-authorization
  format: Bearer scope3_<accessClientId>_<accessClientSecret>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/scope3-ai-openapi-original.yml
  - openapi/_original/scope3-measurement-openapi.yml
  type: http
- alternate_header: x-scope3-api-key
  applies_to: Interchange Buyer + Storefront v2 (api.interchange.io/api/v2/*) and the MCP endpoints
  docs: https://docs.interchange.io/v2/authentication
  format: Bearer scope3_<api_key>
  header: Authorization
  in: header
  name: bearerAuth
  obtain: https://interchange.io/user-api-keys
  probe_evidence:
    note: 'An unauthenticated POST to https://api.interchange.io/mcp/buyer returns HTTP 401 {"error":"Authentication required","message":"API key required. Please provide via x-scope3-api-key header or Authorization: Bearer header"} — observed 2026-08-13.'
  scheme: bearer
  sources:
  - openapi/_original/scope3-buyer-openapi-original.yml
  - openapi/_original/scope3-storefront-openapi-original.yml
  type: http
- authorization_endpoint: https://api.interchange.io/authorize
  discovery: https://api.interchange.io/.well-known/oauth-authorization-server
  dynamic_client_registration: true
  flows:
  - authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.interchange.io
  name: interchange-mcp-oauth
  pkce: S256
  protected_resource: https://api.interchange.io/.well-known/oauth-protected-resource
  registration_endpoint: https://api.interchange.io/auth/register
  role: Recommended path for AI agent connectors (Claude, ChatGPT, Cursor, Codex)
  sources:
  - https://api.interchange.io/.well-known/oauth-authorization-server
  token_endpoint: https://api.interchange.io/auth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
- grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://identity.scope3.com
  name: scope3-identity
  note: Named as a co-equal authorization server in the Interchange protected-resource metadata. client_credentials here is what backs the documented M2M application path.
  openIdConnectUrl: https://identity.scope3.com/.well-known/openid-configuration
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - https://identity.scope3.com/.well-known/openid-configuration
  type: openIdConnect
slug: scope3-authentication
source_filename: scope3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/_original/scope3-ai-openapi-original.yml, openapi/_original/scope3-measurement-openapi.yml,\n  openapi/_original/scope3-buyer-openapi-original.yml, openapi/_original/scope3-storefront-openapi-original.yml,\n  https://api.interchange.io/.well-known/oauth-authorization-server\ndocs:\n- https://docs.scope3.com/docs/access-authorization\n- https://docs.interchange.io/v2/authentication\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_schemes: [bearer]\n  api_key_prefix: scope3_\n  api_key_headers: [Authorization, x-scope3-api-key]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode]\n  identity_provider: WorkOS (https://identity.scope3.com)\n  header: Authorization\n  obtain:\n  - https://interchange.io/user-api-keys\n  - Contact a Scope3 representative for Carbon Calculator / AI Impact Measurement access\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in:\
  \ header\n  header: Authorization\n  format: 'Bearer scope3_<accessClientId>_<accessClientSecret>'\n  docs: https://docs.scope3.com/docs/access-authorization\n  applies_to: Carbon Calculator (api.scope3.com/v2), AI Impact Measurement (aiapi.scope3.com)\n  sources:\n  - openapi/_original/scope3-ai-openapi-original.yml\n  - openapi/_original/scope3-measurement-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer scope3_<api_key>'\n  alternate_header: x-scope3-api-key\n  docs: https://docs.interchange.io/v2/authentication\n  applies_to: Interchange Buyer + Storefront v2 (api.interchange.io/api/v2/*) and the MCP endpoints\n  obtain: https://interchange.io/user-api-keys\n  sources:\n  - openapi/_original/scope3-buyer-openapi-original.yml\n  - openapi/_original/scope3-storefront-openapi-original.yml\n  probe_evidence:\n    note: >-\n      An unauthenticated POST to https://api.interchange.io/mcp/buyer returns HTTP 401\n   \
  \   {\"error\":\"Authentication required\",\"message\":\"API key required. Please provide via\n      x-scope3-api-key header or Authorization: Bearer header\"} — observed 2026-08-13.\n- name: interchange-mcp-oauth\n  type: oauth2\n  role: Recommended path for AI agent connectors (Claude, ChatGPT, Cursor, Codex)\n  discovery: https://api.interchange.io/.well-known/oauth-authorization-server\n  protected_resource: https://api.interchange.io/.well-known/oauth-protected-resource\n  issuer: https://api.interchange.io\n  authorization_endpoint: https://api.interchange.io/authorize\n  token_endpoint: https://api.interchange.io/auth/token\n  registration_endpoint: https://api.interchange.io/auth/register\n  dynamic_client_registration: true\n  pkce: S256\n  flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  sources: ['https://api.interchange.io/.well-known/oauth-authorization-server']\n- name: scope3-identity\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://identity.scope3.com/.well-known/openid-configuration\n  issuer: https://identity.scope3.com\n  scopes: [openid, profile, email, offline_access]\n  grant_types: [authorization_code, client_credentials, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  note: >-\n    Named as a co-equal authorization server in the Interchange protected-resource metadata.\n    client_credentials here is what backs the documented M2M application path.\n  sources: ['https://identity.scope3.com/.well-known/openid-configuration']\ncredential_paths:\n  note: Interchange documents four distinct credential paths, all fronted by WorkOS.\n  paths:\n  - {name: OAuth, audience: interactive connectors and AI agents, mechanism: authorization code + PKCE via MCP connector}\n  - {name: Agent Registration, audience: AI agents, mechanism: dynamic client registration at /auth/register}\n  - {name: Organization API keys, audience: simple customer automation, mechanism: 'scope3_ prefixed\
  \ bearer key'}\n  - {name: M2M applications, audience: backend integrations, mechanism: OAuth client credentials}\nsso:\n  supported: true\n  docs: https://docs.interchange.io/v2/setup/sso-setup\nauthorization:\n  model: role + organization entitlement + persona\n  note: >-\n    No product-level OAuth scopes are published. See scopes/scope3-scopes.yml. A 403 carries\n    FORBIDDEN, ACCESS_DENIED, ALPHA_OPT_IN_REQUIRED or TOS_ACCEPTANCE_REQUIRED, which is where\n    the real authorization surface is visible.\ncross_links:\n  scopes: scopes/scope3-scopes.yml\n  well_known: well-known/scope3-well-known.yml\n  conventions: conventions/scope3-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/authentication/scope3-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Enterprise
- Advertising
- Carbon Emissions
- Sustainability
- AdTech
- Measurements
- Artificial Intelligence
- Agentic
- AdCP
- MCP
- Programmatic
- Media Buying
- Publishing
---
