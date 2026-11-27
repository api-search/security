---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: conveo-ai-interviews-api-openapi.yml
  format: yaml
  label: Conveo Interviews API
  slug: conveo-ai-interviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveo-ai/openapi/conveo-ai-interviews-api-openapi.yml
- filename: conveo-ai-studies-api-openapi.yml
  format: yaml
  label: Conveo Studies API
  slug: conveo-ai-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveo-ai/openapi/conveo-ai-studies-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Conveo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conveo secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conveo
provider_slug: conveo-ai
scheme_count: 4
schemes:
- description: Organization API key supplied as an Authorization Bearer token. "A Bearer token takes precedence when both are supplied." MCP OAuth access tokens are a different credential and are not accepted by REST.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/conveo-ai-openapi.yml
  - https://conveo.ai/docs/api-reference
  surface: REST (https://app.conveo.ai/public-api/v1)
  type: http
- description: Alternative header for the same organization API key.
  in: header
  name: apiKeyAuth
  parameter: Conveo-Api-Key
  sources:
  - openapi/conveo-ai-openapi.yml
  - https://conveo.ai/docs/api-reference
  surface: REST
  type: apiKey
- description: OAuth for interactive assistants on the remote MCP server; the user selects the organization to authorize and tools run as that user. Dynamic client registration accepts supported local callbacks and allowlisted hosted callbacks. A preconfigured public client ID is documented (7326f7bf-48d6-4b75-a418-0c9c0d8eb901) with no client secret. Access tokens expire and are refreshed by compatible clients. No scope list is published.
  name: mcpOAuth
  sources:
  - https://conveo.ai/docs/api-reference/mcp
  surface: MCP (https://app.conveo.ai/api/mcp)
  type: oauth2
- description: An organization API key sent as Bearer exposes exactly six read tools (list_studies, get_study, list_interviews, list_storylines, list_storyline_insights, search_clips); the key acts as its creating user.
  name: mcpApiKey
  scheme: bearer
  sources:
  - https://conveo.ai/docs/api-reference/mcp
  surface: MCP
  type: http
slug: conveo-ai-authentication
source_filename: conveo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://conveo.ai/docs/api-reference\ndocs: https://conveo.ai/docs/api-reference\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: REST (https://app.conveo.ai/public-api/v1)\n  description: 'Organization API key supplied as an Authorization Bearer token. \"A Bearer token takes precedence when both are supplied.\" MCP OAuth access tokens are a different credential and are not accepted by REST.'\n  sources:\n  - openapi/conveo-ai-openapi.yml\n  - https://conveo.ai/docs/api-reference\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Conveo-Api-Key\n  surface: REST\n  description: Alternative header for the same organization API key.\n  sources:\n  - openapi/conveo-ai-openapi.yml\n  - https://conveo.ai/docs/api-reference\n- name: mcpOAuth\n  type: oauth2\n  surface: MCP (https://app.conveo.ai/api/mcp)\n  description:\
  \ OAuth for interactive assistants on the remote MCP server; the user selects the organization to authorize and tools run as that user. Dynamic client registration accepts supported local callbacks and allowlisted hosted callbacks. A preconfigured public client ID is documented (7326f7bf-48d6-4b75-a418-0c9c0d8eb901) with no client secret. Access tokens expire and are refreshed by compatible clients. No scope list is published.\n  sources:\n  - https://conveo.ai/docs/api-reference/mcp\n- name: mcpApiKey\n  type: http\n  scheme: bearer\n  surface: MCP\n  description: An organization API key sent as Bearer exposes exactly six read tools (list_studies, get_study, list_interviews, list_storylines, list_storyline_insights, search_clips); the key acts as its creating user.\n  sources:\n  - https://conveo.ai/docs/api-reference/mcp\nkey_management:\n  issue: Organization admin, Settings → Organization → API keys → Create API key; the key is shown only once.\n  revoke: Delete the key from API keys.\n\
  \  rotate: Create the replacement, update the integration, verify access, then delete the old key.\n  scope: Organization-level access, not the requesting person's study-sharing permissions.\n"
source_yaml_url: https://artifacts.apis.io/conveo-ai/authentication/conveo-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Artificial Intelligence
- Qualitative Research
- Market Research
- Customer Interviews
- Consumer Insights
- MCP
---
