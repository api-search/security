---
api_key_in:
- header
api_specs:
- filename: brainfish-agents-api-openapi.yml
  format: yaml
  label: Brainfish Agents API
  slug: brainfish-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-agents-api-openapi.yml
- filename: brainfish-analytics-api-openapi.yml
  format: yaml
  label: Brainfish Analytics API
  slug: brainfish-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-analytics-api-openapi.yml
- filename: brainfish-authentication-api-openapi.yml
  format: yaml
  label: Brainfish Authentication API
  slug: brainfish-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-authentication-api-openapi.yml
- filename: brainfish-catalogs-api-openapi.yml
  format: yaml
  label: Brainfish Catalogs API
  slug: brainfish-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-catalogs-api-openapi.yml
- filename: brainfish-collections-api-openapi.yml
  format: yaml
  label: Brainfish Collections API
  slug: brainfish-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-collections-api-openapi.yml
- filename: brainfish-conversations-api-openapi.yml
  format: yaml
  label: Brainfish Conversations API
  slug: brainfish-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-conversations-api-openapi.yml
- filename: brainfish-documents-api-openapi.yml
  format: yaml
  label: Brainfish Documents API
  slug: brainfish-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-documents-api-openapi.yml
- filename: brainfish-sessions-api-openapi.yml
  format: yaml
  label: Brainfish Sessions API
  slug: brainfish-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-sessions-api-openapi.yml
- filename: brainfish-users-api-openapi.yml
  format: yaml
  label: Brainfish Users API
  slug: brainfish-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Brainfish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brainfish secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Brainfish
provider_slug: brainfish
scheme_count: 3
schemes:
- bearerFormat: API Token
  description: 'Bearer token authentication. Include your API token in the Authorization header.


    Example: `Authorization: Bearer [example key]`


    Create tokens in your Brainfish dashboard under Settings → API Tokens.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/brainfish-public-api-openapi-original.json
  type: http
- description: '**Deprecated**: Use Bearer authentication instead.


    Legacy access token header for backward compatibility. Must start with `bf_api_`.


    Create tokens in your Brainfish dashboard under Settings → API Tokens.'
  in: header
  name: AccessToken
  parameter: access-token
  sources:
  - openapi/brainfish-public-api-openapi-original.json
  type: apiKey
- description: 'Agent key identifier that specifies which AI agent/widget to use for the request.


    Find agent keys in your Brainfish dashboard under Agents. Click on any agent key to copy it.'
  in: header
  name: AgentKey
  parameter: agent-key
  sources:
  - openapi/brainfish-public-api-openapi-original.json
  type: apiKey
slug: brainfish-authentication
source_filename: brainfish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/brainfish-public-api-openapi-original.json\ndocs: https://docs.brainfi.sh/api-reference\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  description: |-\n    Bearer token authentication. Include your API token in the Authorization header.\n\n    Example: `Authorization: Bearer [example key]`\n\n    Create tokens in your Brainfish dashboard under Settings → API Tokens.\n  sources:\n  - openapi/brainfish-public-api-openapi-original.json\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: access-token\n  description: |-\n    **Deprecated**: Use Bearer authentication instead.\n\n    Legacy access token header for backward compatibility. Must start with `bf_api_`.\n\n    Create tokens in your Brainfish dashboard under Settings → API Tokens.\n  sources:\n  - openapi/brainfish-public-api-openapi-original.json\n\
  - name: AgentKey\n  type: apiKey\n  in: header\n  parameter: agent-key\n  description: |-\n    Agent key identifier that specifies which AI agent/widget to use for the request.\n\n    Find agent keys in your Brainfish dashboard under Agents. Click on any agent key to copy it.\n  sources:\n  - openapi/brainfish-public-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/authentication/brainfish-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- AI
- Customer Support
- Knowledge Base
- Help Desk
- Agents
- Support Automation
- SaaS
---
