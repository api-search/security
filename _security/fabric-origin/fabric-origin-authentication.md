---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: fabric-origin-entertainment-api-openapi.yml
  format: yaml
  label: Fabric Origin Entertainment API
  slug: entertainment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-entertainment-api-openapi.yml
- filename: fabric-origin-celebrity-api-openapi.yml
  format: yaml
  label: Fabric Origin Celebrity API
  slug: celebrity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-celebrity-api-openapi.yml
- filename: fabric-origin-videos-api-openapi.yml
  format: yaml
  label: Fabric Origin Video API
  slug: video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-videos-api-openapi.yml
- filename: fabric-origin-images-api-openapi.yml
  format: yaml
  label: Fabric Origin Image API
  slug: image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-images-api-openapi.yml
- filename: fabric-origin-common-metadata-api-openapi.yml
  format: yaml
  label: Fabric Origin Common Data API
  slug: common-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-common-metadata-api-openapi.yml
- filename: fabric-origin-entertainment-api-openapi.yml
  format: yaml
  label: Fabric Origin Entertainment API
  slug: fabric-origin-entertainment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-entertainment-api-openapi.yml
- filename: fabric-origin-images-api-openapi.yml
  format: yaml
  label: Fabric Origin Images API
  slug: fabric-origin-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-images-api-openapi.yml
- filename: fabric-origin-videos-api-openapi.yml
  format: yaml
  label: Fabric Origin Videos API
  slug: fabric-origin-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-videos-api-openapi.yml
- filename: fabric-origin-video-analytics-api-openapi.yml
  format: yaml
  label: Fabric Origin Video Analytics API
  slug: video-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-video-analytics-api-openapi.yml
- filename: fabric-origin-fandango-api-openapi.yml
  format: yaml
  label: Fabric Origin Fandango API
  slug: fandango-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-fandango-api-openapi.yml
- filename: fabric-origin-captions-translations-api-openapi.yml
  format: yaml
  label: Fabric Origin Captions and Translations API
  slug: captions-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-captions-translations-api-openapi.yml
- filename: fabric-origin-metacritic-api-openapi.yml
  format: yaml
  label: Fabric Origin Metacritic API
  slug: metacritic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-metacritic-api-openapi.yml
- filename: fabric-origin-common-sense-media-api-openapi.yml
  format: yaml
  label: Fabric Origin Common Sense Media API
  slug: common-sense-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-common-sense-media-api-openapi.yml
- filename: fabric-origin-rotten-tomatoes-api-openapi.yml
  format: yaml
  label: Fabric Origin Rotten Tomatoes API
  slug: rotten-tomatoes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rotten-tomatoes-api-openapi.yml
- filename: fabric-origin-rabbit-recommendations-api-openapi.yml
  format: yaml
  label: Fabric Origin Rabbit Recommendations API
  slug: rabbit-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rabbit-recommendations-api-openapi.yml
- filename: fabric-origin-tv-grid-online-api-openapi.yml
  format: yaml
  label: Fabric Origin TV Grid Online API
  slug: tv-grid-online-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-tv-grid-online-api-openapi.yml
- filename: fabric-origin-katch-media-api-openapi.yml
  format: yaml
  label: Fabric Origin Katch Media API
  slug: katch-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-katch-media-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: Fabric Origin runs three distinct authentication models across the Origin family. Origin Nexus (the entertainment metadata REST APIs) uses an Azure API Management subscription key. Origin Studio uses a bearer API key on its JSON:API REST surface. Both Origin MCP servers use OAuth 2.0 with PKCE, each acting as its own authorization server, with an API key accepted as a bearer alternative on Origin Studio MCP for unattended workloads.
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Fabric Origin Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: Fabric Origin secures its APIs with apiKey, http, and oauth2 across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: Fabric Origin
provider_slug: fabric-origin
scheme_count: 0
schemes: []
slug: fabric-origin-authentication
source_filename: fabric-origin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://knowledgebase.fabricdata.com/origin/getting-started\ndocs:\n- https://knowledgebase.fabricdata.com/origin/getting-started\n- https://knowledgebase.fabricdata.com/studio/integrations-and-apis/api-overview/authentication\n- https://knowledgebase.fabricdata.com/studio/origin-studio-mcp-server/origin-studio-mcp-server\n- https://knowledgebase.fabricdata.com/insights/origin-insights-mcp/mcp-access\nprovider: Fabric Origin\nproviderId: fabric-origin\ndescription: >-\n  Fabric Origin runs three distinct authentication models across the Origin family. Origin Nexus\n  (the entertainment metadata REST APIs) uses an Azure API Management subscription key. Origin Studio\n  uses a bearer API key on its JSON:API REST surface. Both Origin MCP servers use OAuth 2.0 with PKCE,\n  each acting as its own authorization server, with an API key accepted as a bearer alternative on\n  Origin Studio MCP for unattended workloads.\nsummary:\n\
  \  types: [apiKey, http, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [authorization_code]\n  pkce: required on both MCP servers (S256 only)\n  note: >-\n    The 14 first-party Origin Nexus OpenAPI documents the provider publishes carry NO\n    components.securitySchemes block. The subscription-key requirement is documented in prose on the\n    getting-started page and is captured here and in overlays/ rather than injected into the\n    provider's spec.\nprofiles:\n- id: origin-nexus\n  name: Origin Nexus entertainment APIs\n  hosts: [api.origin.fabricdata.com, ee.iva-api.com]\n  schemes:\n  - name: SubscriptionKeyHeader\n    type: apiKey\n    in: header\n    parameter: Ocp-Apim-Subscription-Key\n    gateway: Azure API Management\n    source: https://knowledgebase.fabricdata.com/origin/getting-started\n  - name: SubscriptionKeyQuery\n    type: apiKey\n    in: query\n    parameter: subscription-key\n    source: https://knowledgebase.fabricdata.com/origin/getting-started\n   \
  \ note: >-\n      A key in the query string is logged by intermediaries; the header form is the safer of the two\n      the provider offers.\n  key_issuance:\n    self_serve: false\n    portal: https://developer.origin.fabricdata.com/portal/login\n    trial: 30-day free trial requested through https://www.fabricdata.com/contact-us\n    note: Keys are retrieved from the Origin Service Portal once a subscription exists.\n  server_to_server: true\n- id: origin-studio-rest\n  name: Origin Studio Production API\n  hosts: [api.studio.fabricdata.com, api.stg.studio.fabricdata.com]\n  schemes:\n  - name: StudioApiKey\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Authorization: Bearer YOUR_API_KEY'\n    source: https://knowledgebase.fabricdata.com/studio/integrations-and-apis/api-overview/authentication\n  key_issuance:\n    self_serve: false\n    issued_by: [Origin Studio administrator, Fabric Support]\n    admin_path: Administrator -> Security -> API Keys -> Generate\
  \ Key\n  required_headers: ['Authorization: Bearer <key>', 'Accept: application/json', 'Content-Type: application/json (POST/PUT/PATCH)']\n- id: origin-studio-mcp\n  name: Origin Studio MCP Server\n  hosts: [mcp-api.studio.fabricdata.com]\n  schemes:\n  - name: StudioMcpOAuth\n    type: oauth2\n    flow: authorization_code\n    pkce: required (S256 only; `plain` and missing code_challenge are rejected)\n    client_auth: none (public clients)\n    issuer: https://mcp-api.studio.fabricdata.com\n    authorization_endpoint: https://mcp-api.studio.fabricdata.com/authorize\n    token_endpoint: https://mcp-api.studio.fabricdata.com/token\n    registration_endpoint: https://mcp-api.studio.fabricdata.com/register\n    dynamic_client_registration: true\n    scopes: [openid, profile, email, offline_access]\n    refresh_tokens: 'issued with offline_access; long-lived and NON-ROTATING — the provider explicitly warns to store them encrypted and revoke on offboarding'\n    organization_selection: required\
  \ at login; a client cannot pre-select the tenant\n    discovery: https://mcp-api.studio.fabricdata.com/.well-known/oauth-authorization-server\n    probed_status: 200\n  - name: StudioMcpApiKey\n    type: http\n    scheme: bearer\n    note: >-\n      Any non-JWT bearer is treated as an Origin Studio API key and validated server-side. This is\n      the supported headless path; there is no client-credentials flow for third parties.\n  protected_resource_metadata: https://mcp-api.studio.fabricdata.com/.well-known/oauth-protected-resource\n  challenge: 'HTTP 401 with WWW-Authenticate: Bearer error=\"invalid_token\", resource_metadata=<RFC 9728 URL>'\n  broker_note: >-\n    Origin Studio brokers login with Auth0 internally but the MCP server is its own authorization\n    server. Clients never talk to Auth0 directly; Auth0 DCR is disabled and rejects registration.\n- id: origin-insights-mcp\n  name: Origin Insights MCP Server\n  hosts: [insights.fabric-mcp.link]\n  schemes:\n  - name: InsightsMcpOAuth\n\
  \    type: oauth2\n    flow: authorization_code\n    issuer: https://insights.fabric-mcp.link/\n    authorization_endpoint: https://insights.fabric-mcp.link/oauth/authorize\n    token_endpoint: https://insights.fabric-mcp.link/oauth/token\n    registration_endpoint: https://insights.fabric-mcp.link/oauth/register\n    jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_V84pL7JUo/.well-known/jwks.json\n    dynamic_client_registration: true\n    scopes: [openid, email, profile]\n    discovery: https://insights.fabric-mcp.link/.well-known/oauth-authorization-server\n    probed_status: 200\n  protected_resource_metadata: https://insights.fabric-mcp.link/.well-known/oauth-protected-resource\n  challenge: 'HTTP 401 with WWW-Authenticate: Bearer realm=\"fabric-mcp\", resource_metadata=<RFC 9728 URL>'\ngovernance:\n  source: https://www.fabricdata.com/agent-governance\n  machine_identity: agents authenticate as first-class OAuth identities; service accounts supported\n  no_shared_human_credentials:\
  \ true\n  rbac: agent permissions map to the same RBAC model that governs human users\n  audit: agent actions are logged and attributable to the acting identity\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/authentication/fabric-origin-authentication.yml
summary_line: apiKey/http/oauth2 · 0 schemes
tags:
- Entertainment
- Metadata
- Movies
- Television
- Games
- Celebrities
- Trailers
- Images
- TV Listings
- Market Intelligence
- Media
- MCP
---
