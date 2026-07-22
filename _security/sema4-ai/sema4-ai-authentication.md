---
api_key_in:
- header
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Sema4 Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sema4 Ai secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sema4 Ai
provider_slug: sema4-ai
scheme_count: 3
schemes:
- description: 'The Sema4.ai REST API (v2) and Work Item API (v1) authenticate with a platform API key sent as a bearer token: `Authorization: Bearer YOUR_API_KEY`. API keys are created and managed in the application under Configuration > API Keys (Control Room), scoped per Workspace, and shown only once at creation.'
  format: Bearer <api_key>
  header: Authorization
  name: apiKeyBearer
  scheme: bearer
  sources:
  - docs
  type: http
- description: 'Team Edition running as a Snowflake Native App accepts a Snowflake token: `Authorization: Snowflake Token="<token>"`.'
  name: snowflakeToken
  scheme: bearer
  sources:
  - docs
  type: http
- description: The platform exposes an OIDC surface (see /api/v2/oidc) for enterprise SSO identity integration; used for user authentication into Control Room / Work Room.
  name: oidc
  sources:
  - docs
  type: openIdConnect
slug: sema4-ai-authentication
source_filename: sema4-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://sema4.ai/docs/v2/api + https://sema4.ai/docs/work-item-api\ndocs: https://sema4.ai/docs/v2/api/api-keys\nsummary:\n  types: [http, openIdConnect]\n  api_key_in: [header]\n  scheme: bearer\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  description: >-\n    The Sema4.ai REST API (v2) and Work Item API (v1) authenticate with a\n    platform API key sent as a bearer token: `Authorization: Bearer YOUR_API_KEY`.\n    API keys are created and managed in the application under Configuration >\n    API Keys (Control Room), scoped per Workspace, and shown only once at creation.\n  header: Authorization\n  format: Bearer <api_key>\n  sources: [docs]\n- name: snowflakeToken\n  type: http\n  scheme: bearer\n  description: >-\n    Team Edition running as a Snowflake Native App accepts a Snowflake token:\n    `Authorization: Snowflake Token=\"<token>\"`.\n  sources: [docs]\n- name: oidc\n  type: openIdConnect\n\
  \  description: >-\n    The platform exposes an OIDC surface (see /api/v2/oidc) for enterprise SSO\n    identity integration; used for user authentication into Control Room / Work Room.\n  sources: [docs]\nnotes: >-\n  The GET on the API base (`/api/v2`) returns the deployment's OpenAPI spec with\n  no API key required; all other endpoints require the bearer API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sema4-ai/refs/heads/main/authentication/sema4-ai-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- MCP
- Enterprise AI
- Actions
- Python
- Developer Tools
---
