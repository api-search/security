---
api_key_in:
- query
- header
api_specs:
- filename: nexla-rest-api-openapi.yml
  format: yaml
  label: Nexla REST API
  slug: nexla-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/openapi/nexla-rest-api-openapi.yml
- filename: nexla-genai-mcpaas-openapi.json
  format: json
  label: Nexla GenAI API (RAG + MCPaaS)
  slug: nexla-genai-api-rag-mcpaas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/openapi/nexla-genai-mcpaas-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nexla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nexla secures its APIs with http and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nexla
provider_slug: nexla
scheme_count: 6
schemes:
- applies_to: Top-level security on the Nexla REST API — every operation unless overridden.
  bearerFormat: JWT
  default: true
  name: NexlaSessionToken
  scheme: Bearer
  sources:
  - openapi/nexla-rest-api-openapi.yml
  type: http
- applies_to: Webhook ingestion operations (send_one_record, send_many_records).
  in: query
  name: NexlaApiKeyQuery
  parameter: api_key
  sources:
  - openapi/nexla-rest-api-openapi.yml
  type: apiKey
- applies_to: Webhook ingestion operations, as the header alternative to the query key.
  name: NexlaApiKeyHeader
  scheme: Basic
  sources:
  - openapi/nexla-rest-api-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/nexla-rest-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: The token that is used when logging into Nexla via Google SSO.
  name: GoogleSSOToken
  scheme: Bearer
  sources:
  - openapi/nexla-rest-api-openapi.yml
  type: http
- applies_to: Nexla GenAI (RAG + MCPaaS) API and the remote MCP endpoint.
  name: NexlaServiceKey
  note: The published GenAI OpenAPI declares an EMPTY securitySchemes map even though every operation requires authentication. This scheme comes from the docs and is added by our overlay, not invented.
  scheme: bearer
  sources:
  - docs
  - overlays/nexla-genai-mcpaas-overlay.yaml
  type: http
slug: nexla-authentication
source_filename: nexla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://docs.nexla.com/dev-guides/authentication/overview and\n  https://docs.nexla.com/dev-guides/authentication (docs) enriched over the securitySchemes derived from\n  openapi/nexla-rest-api-openapi.yml\ndocs: https://docs.nexla.com/dev-guides/authentication\nsummary:\n  types:\n  - http\n  - apiKey\n  oauth2: false\n  openid_connect: partial\n  mutual_tls: false\n  api_key_in:\n  - query\n  - header\n  transport: 'HTTPS only — \"Calls made without authentication or over plain HTTP will fail with HTTP status 401 (Unauthorized)\"'\n  accept_header: 'Accept: application/vnd.nexla.api.v1+json'\ncredential_models:\n- name: Session access token\n  kind: bearer-jwt\n  lifetime: '~1 hour (configurable)'\n  obtained_from:\n  - 'Nexla UI /token route — e.g. https://dataops.nexla.io/token — which routes through the org preferred Identity Provider'\n  - Nexla CLI\n  - exchange from a service key\n  usage: 'Authorization: Bearer\
  \ <access-token>'\n  purpose: 'Interactive API usage and CLI operations; development, testing and manual API exploration.'\n  refresh: 'NexlaClient.refresh_access_token() in the Python SDK; re-exchange the service key otherwise.'\n- name: Service key\n  kind: long-lived-secret\n  lifetime: 'permanent (until rotated or deactivated)'\n  obtained_from:\n  - Nexla UI\n  - Nexla API\n  usage: 'Exchanged for a session token, or sent as Bearer to the GenAI/MCP surface.'\n  purpose: 'Server-to-server communication, automated workflows, integration scenarios, and MCP server authentication.'\n- name: Per-resource API key\n  kind: resource-scoped-key\n  lifetime: 'until rotated via the API key management endpoints'\n  usage:\n  - 'Authorization: Basic <api-key>'\n  - '?api_key=<api-key>'\n  purpose: 'Authenticating a specific resource — notably the webhook ingestion endpoints.'\n  warning: 'Docs: \"Never share your API keys. Keep them guarded and secure. If you think the key has been compromised,\
  \ you can rotate the API key by calling relevant API Key management endpoints.\"'\nschemes:\n- name: NexlaSessionToken\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  default: true\n  applies_to: 'Top-level security on the Nexla REST API — every operation unless overridden.'\n  sources: [openapi/nexla-rest-api-openapi.yml]\n- name: NexlaApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  applies_to: 'Webhook ingestion operations (send_one_record, send_many_records).'\n  sources: [openapi/nexla-rest-api-openapi.yml]\n- name: NexlaApiKeyHeader\n  type: http\n  scheme: Basic\n  applies_to: 'Webhook ingestion operations, as the header alternative to the query key.'\n  sources: [openapi/nexla-rest-api-openapi.yml]\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources: [openapi/nexla-rest-api-openapi.yml]\n- name: GoogleSSOToken\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: 'The token that is used when logging into Nexla via Google SSO.'\n\
  \  sources: [openapi/nexla-rest-api-openapi.yml]\n- name: NexlaServiceKey\n  type: http\n  scheme: bearer\n  applies_to: 'Nexla GenAI (RAG + MCPaaS) API and the remote MCP endpoint.'\n  sources: [docs, overlays/nexla-genai-mcpaas-overlay.yaml]\n  note: >-\n    The published GenAI OpenAPI declares an EMPTY securitySchemes map even though every operation requires\n    authentication. This scheme comes from the docs and is added by our overlay, not invented.\noauth:\n  rest_api: false\n  mcp: true\n  detail: >-\n    The REST API does not use OAuth. The MCP surface does, for clients that cannot send a custom header.\n    RFC 9728 Protected Resource Metadata is served at\n    https://api-genai.nexla.io/.well-known/oauth-protected-resource with scopes_supported\n    [openid, email, profile] and bearer_methods_supported [header]. Upstream identity bridges are\n    declared in the GenAI contract at /mcp/auth/google/callback and /mcp/auth/azure/callback.\n  scopes_artifact: null\n  scopes_note:\
  \ >-\n    No `scopes/` artifact is emitted. derive-oauth-scopes.py found zero oauth2 securitySchemes in either\n    contract, and the only scopes Nexla publishes are the three standard OIDC scopes above — an identity\n    surface, not an API permission model. Nexla's authorization model is role-based accessors\n    (AccessRoles bound per resource), not OAuth scopes.\nenterprise_sso:\n  supported: true\n  protocols: [OIDC, 'SAML 2.0']\n  tier: Enterprise\n  api_surface:\n  - 'GET /orgs/{org_id}/auth_settings (get_api_auth_settings)'\n  - 'PUT /orgs/{org_id}/auth_settings/{auth_setting_id} (update_api_auth_config)'\n  - 'GET|POST /api_auth_configs (get_api_auth_configs, create_api_auth_config)'\n  fields_declared: [oidc_domain, oidc_keys_url_key, oidc_id_claims, oidc_access_claims, oidc_token_verify_url, idp_entity_id, service_entity_id]\n  source: https://nexla.com/pricing/\nsecurity_best_practices_docs: https://docs.nexla.com/dev-guides/authentication/security-best-practices\nevidence:\n\
  - url: https://docs.nexla.com/dev-guides/authentication/overview\n  status: 200\n- url: https://dataops.nexla.io/nexla-api/teams\n  status: 401\n  note: 'live unauthenticated probe confirms auth is enforced'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexla/refs/heads/main/authentication/nexla-authentication.yml
summary_line: http/apiKey · 6 schemes
tags:
- Company
- Data Integration
- Data Engineering
- ETL
- ELT
- Data Products
- Streaming
- Change Data Capture
- Data Governance
- Artificial Intelligence
- Retrieval Augmented Generation
- MCP
- Agent Tools
- Data Pipelines
- Connectors
---
