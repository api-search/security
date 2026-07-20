---
api_key_in:
- header
api_specs:
- filename: duvo-ai-openapi-original.json
  format: json
  label: Duvo Public API
  slug: duvo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duvo-ai/refs/heads/main/openapi/duvo-ai-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Duvo Ai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Duvo Ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Duvo Ai
provider_slug: duvo-ai
scheme_count: 2
schemes:
- description: 'Workspace-issued bearer API token. Sent as Authorization: Bearer <token>. Get an API key from the Duvo dashboard (provisioned per approved workspace).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/duvo-ai-openapi-original.json
  type: http
- authorization_server: https://login.duvo.ai/.well-known/oauth-authorization-server
  description: 'Scoped OAuth client credentials for enterprise workspaces where Duvo has enabled OAuth for the customer tenant. Access token used as Authorization: Bearer <access_token>. Not declared in the public OpenAPI; documented at https://www.duvo.ai/auth.md and discoverable via RFC 9728 protected-resource metadata + RFC 8414 authorization-server metadata.'
  flow: clientCredentials
  name: oauth2ClientCredentials
  protected_resource_metadata: https://api.duvo.ai/.well-known/oauth-protected-resource
  sources:
  - https://www.duvo.ai/auth.md
  - well-known/duvo-ai-oauth-protected-resource.json
  - well-known/duvo-ai-oauth-authorization-server.json
  token_url: https://login.duvo.ai/oauth/token
  type: oauth2
slug: duvo-ai-authentication
source_filename: duvo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/duvo-ai-openapi-original.json\ndocs: https://www.duvo.ai/auth.md\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Duvo access is workspace-scoped. The public OpenAPI declares a single http\n    bearer scheme (workspace-issued API tokens). The docs auth guide additionally\n    documents scoped OAuth client credentials for enterprise workspaces where Duvo\n    has enabled OAuth for the tenant, plus SSO/RBAC for human users and managed\n    OAuth/API connections for third-party business systems. Public self-serve\n    dynamic agent registration is NOT available; API/MCP/OAuth/sandbox access is\n    provisioned by Duvo during an approved customer or pilot onboarding.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Workspace-issued bearer API token. Sent as Authorization: Bearer <token>.\n    Get an API key\
  \ from the Duvo dashboard (provisioned per approved workspace).\n  sources:\n  - openapi/duvo-ai-openapi-original.json\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://login.duvo.ai/oauth/token\n  authorization_server: https://login.duvo.ai/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://api.duvo.ai/.well-known/oauth-protected-resource\n  description: >-\n    Scoped OAuth client credentials for enterprise workspaces where Duvo has\n    enabled OAuth for the customer tenant. Access token used as\n    Authorization: Bearer <access_token>. Not declared in the public OpenAPI;\n    documented at https://www.duvo.ai/auth.md and discoverable via RFC 9728\n    protected-resource metadata + RFC 8414 authorization-server metadata.\n  sources:\n  - https://www.duvo.ai/auth.md\n  - well-known/duvo-ai-oauth-protected-resource.json\n  - well-known/duvo-ai-oauth-authorization-server.json\nerror_semantics:\n  status_401: missing,\
  \ expired, malformed, or revoked credentials\n  status_403: insufficient scope, workspace policy denial, RBAC denial, or human approval requirement\n  documented_error_ids:\n  - invalid_token\n  - insufficient_scope\n  - workspace_policy_denied\n  - approval_required\n  - rate_limited\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duvo-ai/refs/heads/main/authentication/duvo-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise; Ai
- Process Intelligence
- Automation
- Agents
- SAP Migration
- Operations
- ERP
- Transformation
- Approvals
- Audit
- MCP
---
