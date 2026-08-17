---
api_key_in:
- header
api_specs:
- filename: ada-subpackage-channels-api-openapi.yml
  format: yaml
  label: Ada subpackage_channels API
  slug: ada-subpackage-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-channels-api-openapi.yml
- filename: ada-subpackage-conversations-api-openapi.yml
  format: yaml
  label: Ada subpackage_conversations API
  slug: ada-subpackage-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-conversations-api-openapi.yml
- filename: ada-subpackage-deletechatterdata-api-openapi.yml
  format: yaml
  label: Ada subpackage_deleteChatterData API
  slug: ada-subpackage-deletechatterdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-deletechatterdata-api-openapi.yml
- filename: ada-subpackage-endusers-api-openapi.yml
  format: yaml
  label: Ada subpackage_endUsers API
  slug: ada-subpackage-endusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-endusers-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-articles-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/articles API
  slug: ada-subpackage-knowledge-subpackage-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-articles-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-sources-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/sources API
  slug: ada-subpackage-knowledge-subpackage-knowledge-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-sources-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-tags-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/tags API
  slug: ada-subpackage-knowledge-subpackage-knowledge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-tags-api-openapi.yml
- filename: ada-subpackage-messages-api-openapi.yml
  format: yaml
  label: Ada subpackage_messages API
  slug: ada-subpackage-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-messages-api-openapi.yml
- filename: ada-subpackage-platformintegrations-api-openapi.yml
  format: yaml
  label: Ada subpackage_platformIntegrations API
  slug: ada-subpackage-platformintegrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-platformintegrations-api-openapi.yml
- filename: ada-subpackage-webhookmanagement-api-openapi.yml
  format: yaml
  label: Ada subpackage_webhookManagement API
  slug: ada-subpackage-webhookmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-webhookmanagement-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ada Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Ada secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Ada
provider_slug: ada
scheme_count: 3
schemes:
- credential: Ada API key
  header: 'Authorization: Bearer <api-key>'
  in_openapi: true
  legacy:
    note: Per-API "(Legacy)" keys still exist and work ONLY against v1 endpoints. They cannot be renamed and will 401 against v2.
  name: bearerAuth
  properties:
    display: the key value is shown once at creation and never again
    expiry: none — keys remain valid until manually revoked
    generation: Ada dashboard — Config > PLATFORM > API keys (generative) or Settings > Integrations > APIs (scripted)
    permissions: read AND write across every API the organization has access to; no per-key scoping
    rotation: multiple concurrent keys supported, so keys can be rotated without downtime
  scheme: bearer
  security_observation: Ada's API keys are non-expiring, unscoped and grant full read/write. There is no read-only key, no per-resource scoping and no key TTL. An agent handed an Ada key holds every permission the organization has.
  sources:
  - openapi/_original/ada-data-compliance-openapi.yml
  - openapi/_original/ada-data-export-openapi.yml
  - openapi/_original/ada-data-export-v1-4-openapi.yml
  - openapi/_original/ada-knowledge-openapi.yml
  type: http
- artifact: scopes/ada-scopes.yml
  audience: partner-built platform integrations installed into a customer AI Agent
  flows:
  - flow: authorizationCode
    scopes: 8
    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token
  - flow: refreshToken
    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token
  in_openapi: false
  name: PlatformIntegrationsOAuth
  sources:
  - https://docs.ada.cx/reference/integrations/getting-started
  token_lifetimes:
    access_token: 1 hour
    authorization_code: 5 minutes
    refresh_token: 30 days (rotated on every use)
  type: oauth2
- authorization_model: role-based, not scope-based
  endpoint: https://<your-ada-instance-domain>/api/mcp/oauth
  in_openapi: false
  name: MCPOAuth
  note: Role changes apply on the next tool call. Write tools are hidden from the assistant's tool list for read-only roles. The API-key MCP endpoint (/api/mcp) uses a separate auth path scoped by the key's permissions, which — per the key model above — is effectively full access.
  roles:
    Admin: all tools, including writes
    Agent: read-only tools
    Owner: all tools, including writes
    Read Only: read-only tools
  sources:
  - https://docs.ada.cx/mcp/introduction/authentication
  type: oauth2
slug: ada-authentication
source_filename: ada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\ndocs: https://docs.ada.cx/reference/introduction/authentication\nsource: >-\n  https://docs.ada.cx/reference/introduction/authentication,\n  https://docs.ada.cx/reference/integrations/getting-started,\n  https://docs.ada.cx/mcp/introduction/authentication,\n  openapi/_original/ada-data-compliance-openapi.yml,\n  openapi/_original/ada-data-export-openapi.yml,\n  openapi/_original/ada-data-export-v1-4-openapi.yml,\n  openapi/_original/ada-knowledge-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  api_key_in:\n  - header\n  note: >-\n    The published OpenAPI documents declare exactly one scheme — http/bearer. The docs add a\n    second, spec-invisible model: OAuth 2.0 for partner platform integrations. A third path,\n    dashboard-role-scoped OAuth, governs the MCP server. All three are recorded here.\nschemes:\n- name: bearerAuth\n  type:\
  \ http\n  scheme: bearer\n  in_openapi: true\n  sources:\n  - openapi/_original/ada-data-compliance-openapi.yml\n  - openapi/_original/ada-data-export-openapi.yml\n  - openapi/_original/ada-data-export-v1-4-openapi.yml\n  - openapi/_original/ada-knowledge-openapi.yml\n  credential: Ada API key\n  header: 'Authorization: Bearer <api-key>'\n  properties:\n    expiry: none — keys remain valid until manually revoked\n    rotation: multiple concurrent keys supported, so keys can be rotated without downtime\n    permissions: read AND write across every API the organization has access to; no per-key scoping\n    display: the key value is shown once at creation and never again\n    generation: Ada dashboard — Config > PLATFORM > API keys (generative) or Settings > Integrations > APIs (scripted)\n  legacy:\n    note: >-\n      Per-API \"(Legacy)\" keys still exist and work ONLY against v1 endpoints. They cannot be\n      renamed and will 401 against v2.\n  security_observation: >-\n    Ada's API\
  \ keys are non-expiring, unscoped and grant full read/write. There is no read-only\n    key, no per-resource scoping and no key TTL. An agent handed an Ada key holds every\n    permission the organization has.\n- name: PlatformIntegrationsOAuth\n  type: oauth2\n  in_openapi: false\n  sources:\n  - https://docs.ada.cx/reference/integrations/getting-started\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token\n    scopes: 8\n  - flow: refreshToken\n    tokenUrl: https://{bot-handle}.ada.support/api/platform_integrations/oauth/token\n  token_lifetimes:\n    authorization_code: 5 minutes\n    access_token: 1 hour\n    refresh_token: 30 days (rotated on every use)\n  audience: partner-built platform integrations installed into a customer AI Agent\n  artifact: scopes/ada-scopes.yml\n- name: MCPOAuth\n  type: oauth2\n  in_openapi: false\n  sources:\n  - https://docs.ada.cx/mcp/introduction/authentication\n  endpoint: https://<your-ada-instance-domain>/api/mcp/oauth\n\
  \  authorization_model: role-based, not scope-based\n  roles:\n    Owner: all tools, including writes\n    Admin: all tools, including writes\n    Agent: read-only tools\n    Read Only: read-only tools\n  note: >-\n    Role changes apply on the next tool call. Write tools are hidden from the assistant's tool\n    list for read-only roles. The API-key MCP endpoint (/api/mcp) uses a separate auth path\n    scoped by the key's permissions, which — per the key model above — is effectively full access.\nhost_model:\n  note: >-\n    Credentials are scoped to one Ada instance. The host itself is the tenant boundary:\n    <handle>.ada.support, with regional/cluster variants <handle>.eu.ada.support,\n    <handle>.maple.ada.support, <handle>.us2.ada.support.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/authentication/ada-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- ai
- customer-service
- chatbot
- automation
- conversational-ai
- helpdesk
- crm
- integrations
- knowledge-management
- data-export
---
