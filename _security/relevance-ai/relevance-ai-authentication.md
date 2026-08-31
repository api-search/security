---
api_key_in:
- header
api_specs:
- filename: relevance-ai-openapi.json
  format: json
  label: Relevance AI API
  slug: relevance-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/openapi/relevance-ai-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Relevance Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Relevance AI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Relevance AI
provider_slug: relevance-ai
scheme_count: 2
schemes:
- applied_globally: true
  description: 'Authorization credentials. Header authorization should be in the form of: project:api_key'
  detail: Declared as the single global security requirement in the spec, so every one of the 566 operations is gated by it.
  in: header
  name: AuthorizationHeader
  parameter: Authorization
  sources:
  - openapi/relevance-ai-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://mcp.relevanceai.com/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://mcp.relevanceai.com/token
    registrationUrl: https://mcp.relevanceai.com/register
    revocationUrl: https://mcp.relevanceai.com/revoke
    scopes:
      claudeai: The only advertised scope; authorization is really carried by project role.
    tokenUrl: https://mcp.relevanceai.com/token
  name: MCP OAuth 2.0
  sources:
  - https://mcp.relevanceai.com/.well-known/oauth-authorization-server
  - https://mcp.relevanceai.com/.well-known/oauth-protected-resource
  surface: https://mcp.relevanceai.com/
  type: oauth2
slug: relevance-ai-authentication
source_filename: relevance-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  openapi/relevance-ai-openapi.json (derived baseline) upgraded from\n  https://relevanceai.com/docs/sdk/authentication and\n  https://mcp.relevanceai.com/.well-known/oauth-authorization-server\ndocs: https://relevanceai.com/docs/sdk/authentication\nprovider: Relevance AI\nproviderId: relevance-ai\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  surfaces:\n    rest: apiKey header\n    mcp: oauth2 authorization_code + PKCE\nschemes:\n  - name: AuthorizationHeader\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: 'Authorization credentials. Header authorization should be in the form of: project:api_key'\n    sources:\n      - openapi/relevance-ai-openapi.json\n    applied_globally: true\n    detail: >-\n      Declared as the single global security requirement in the spec, so every one of the 566\n      operations is gated by it.\n  - name: MCP OAuth 2.0\n    type:\
  \ oauth2\n    surface: https://mcp.relevanceai.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.relevanceai.com/authorize\n        tokenUrl: https://mcp.relevanceai.com/token\n        refreshUrl: https://mcp.relevanceai.com/token\n        revocationUrl: https://mcp.relevanceai.com/revoke\n        registrationUrl: https://mcp.relevanceai.com/register\n        pkce: S256\n        scopes:\n          claudeai: The only advertised scope; authorization is really carried by project role.\n    sources:\n      - https://mcp.relevanceai.com/.well-known/oauth-authorization-server\n      - https://mcp.relevanceai.com/.well-known/oauth-protected-resource\ncredential_types:\n  - name: API key\n    format: 'sk-...'\n    header_form: 'Authorization: <project_id>:<api_key>'\n    scope: full access to every resource in the project\n    environment: server-side only\n    expiry: >-\n      Does not auto-expire. \"Existing keys do not auto-expire and must be manually\n\
  \      decommissioned via the dashboard to terminate access.\"\n    rotation: manual, via the dashboard\n    warning: >-\n      The provider warns explicitly against embedding API keys in client-side code,\n      browser-accessible environment variables, or version control.\n  - name: Embed key\n    generated: at runtime via Key.generateEmbedKey()\n    scope: exactly one public agent OR one workforce\n    environment: browser-safe\n    persistence: >-\n      Serialize with key.toJSON() and restore via the Key constructor. Regenerating on every\n      page load breaks conversation continuity, because a key initializes a user session.\n    constraint: The target agent must be marked public; private agents are not reachable with an embed key.\n  - name: MCP OAuth token\n    obtained_via: browser consent flow, per project\n    scope: bounded by the caller's project role; Run-Only mode strips write tools server-side\nregions:\n  required: true\n  detail: >-\n    The client must select the region\
  \ its project lives in. Region is part of the API hostname,\n    so an otherwise valid key against the wrong regional host will not work.\n  values:\n    REGION_US: bcbe5a\n    REGION_EU: d7b62b\n    REGION_AU: f1db6c\ncross_links:\n  scopes: scopes/relevance-ai-scopes.yml\n  conventions: conventions/relevance-ai-conventions.yml\n  mcp: mcp/relevance-ai-mcp.yml\ngaps:\n  - No OAuth on the REST API; API keys are the only server-side credential.\n  - No key scoping or least-privilege on REST — a key is project-wide.\n  - No documented key expiry or forced rotation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/authentication/relevance-ai-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI Agents
- AI Automation
- Multi-Agent Systems
- Agent Platform
- MCP
- agent-native
- Workflow-Automation
- LLM Orchestration
- Knowledge-Management
- Observability
- Sales Automation
- GTM Engineering
---
