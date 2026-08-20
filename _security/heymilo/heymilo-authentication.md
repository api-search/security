---
api_key_in:
- header
api_specs:
- filename: heymilo-ats-api-openapi.yml
  format: yaml
  label: HeyMilo ATS API
  slug: heymilo-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-ats-api-openapi.yml
- filename: heymilo-candidates-api-openapi.yml
  format: yaml
  label: HeyMilo Candidates API
  slug: heymilo-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-candidates-api-openapi.yml
- filename: heymilo-design-template-groups-api-openapi.yml
  format: yaml
  label: HeyMilo Design Template Groups API
  slug: heymilo-design-template-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-design-template-groups-api-openapi.yml
- filename: heymilo-design-templates-api-openapi.yml
  format: yaml
  label: HeyMilo Design Templates API
  slug: heymilo-design-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-design-templates-api-openapi.yml
- filename: heymilo-domains-api-openapi.yml
  format: yaml
  label: HeyMilo Domains API
  slug: heymilo-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-domains-api-openapi.yml
- filename: heymilo-email-template-groups-api-openapi.yml
  format: yaml
  label: HeyMilo Email Template Groups API
  slug: heymilo-email-template-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-email-template-groups-api-openapi.yml
- filename: heymilo-email-templates-api-openapi.yml
  format: yaml
  label: HeyMilo Email Templates API
  slug: heymilo-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-email-templates-api-openapi.yml
- filename: heymilo-health-api-openapi.yml
  format: yaml
  label: HeyMilo Health API
  slug: heymilo-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-health-api-openapi.yml
- filename: heymilo-interview-templates-api-openapi.yml
  format: yaml
  label: HeyMilo Interview Templates API
  slug: heymilo-interview-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-interview-templates-api-openapi.yml
- filename: heymilo-interviewers-api-openapi.yml
  format: yaml
  label: HeyMilo Interviewers API
  slug: heymilo-interviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-interviewers-api-openapi.yml
- filename: heymilo-interviews-api-openapi.yml
  format: yaml
  label: HeyMilo Interviews API
  slug: heymilo-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-interviews-api-openapi.yml
- filename: heymilo-phone-numbers-api-openapi.yml
  format: yaml
  label: HeyMilo Phone Numbers API
  slug: heymilo-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-phone-numbers-api-openapi.yml
- filename: heymilo-questions-api-openapi.yml
  format: yaml
  label: HeyMilo Questions API
  slug: heymilo-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-questions-api-openapi.yml
- filename: heymilo-schema-discovery-api-openapi.yml
  format: yaml
  label: HeyMilo Schema Discovery API
  slug: heymilo-schema-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-schema-discovery-api-openapi.yml
- filename: heymilo-sender-emails-api-openapi.yml
  format: yaml
  label: HeyMilo Sender Emails API
  slug: heymilo-sender-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-sender-emails-api-openapi.yml
- filename: heymilo-voices-api-openapi.yml
  format: yaml
  label: HeyMilo Voices API
  slug: heymilo-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-voices-api-openapi.yml
- filename: heymilo-webhooks-api-openapi.yml
  format: yaml
  label: HeyMilo Webhooks API
  slug: heymilo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-webhooks-api-openapi.yml
- filename: heymilo-workspaces-api-openapi.yml
  format: yaml
  label: HeyMilo Workspaces API
  slug: heymilo-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Heymilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeyMilo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HeyMilo
provider_slug: heymilo
scheme_count: 2
schemes:
- description: API key for authentication. Pass your key in the X-API-KEY header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/heymilo-openapi-original.json
  type: apiKey
- applies_to: https://mcp.heymilo.ai/mcp
  description: MCP server bearer token — either an OAuth 2.1 access token (authorization_code + PKCE S256, refresh_token; scopes openid, profile, email, offline_access) or a HeyMilo API key. OAuth server metadata is published at https://mcp.heymilo.ai/.well-known/oauth-authorization-server.
  name: MCPBearer
  scheme: bearer
  sources:
  - https://docs.heymilo.ai/api-reference/mcp/getting-started
  - well-known/heymilo-oauth-authorization-server.json
  type: http
slug: heymilo-authentication
source_filename: heymilo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/heymilo-openapi-original.json\ndocs: https://docs.heymilo.ai/api-reference/public-api/documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    The HeyMilo Public REST API authenticates every request with an X-API-KEY\n    header. One API key maps to one workspace, is shared per workspace, and does\n    not expire. Requests without a valid key return 401 Unauthorized. The\n    separate hosted MCP server (https://mcp.heymilo.ai/mcp) additionally accepts\n    OAuth 2.1 (Sign in with HeyMilo) or an API key, both passed as\n    Authorization: Bearer <token>.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key for authentication. Pass your key in the X-API-KEY header.\n  sources:\n  - openapi/heymilo-openapi-original.json\n- name: MCPBearer\n  type: http\n  scheme: bearer\n  applies_to: https://mcp.heymilo.ai/mcp\n  description: >-\n\
  \    MCP server bearer token — either an OAuth 2.1 access token (authorization_code\n    + PKCE S256, refresh_token; scopes openid, profile, email, offline_access) or\n    a HeyMilo API key. OAuth server metadata is published at\n    https://mcp.heymilo.ai/.well-known/oauth-authorization-server.\n  sources:\n  - https://docs.heymilo.ai/api-reference/mcp/getting-started\n  - well-known/heymilo-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/authentication/heymilo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Recruiting
- Hiring
- Human Resources
- HR Tech
- Artificial Intelligence
- AI Agents
- Interviewing
- Candidate Screening
- Voice AI
- Webhook
- ATS Integration
---
