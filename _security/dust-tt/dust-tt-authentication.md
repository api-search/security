---
api_key_in: []
api_specs:
- filename: dust-tt-agents-api-openapi.yml
  format: yaml
  label: Dust Agents API
  slug: dust-tt-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-agents-api-openapi.yml
- filename: dust-tt-apps-api-openapi.yml
  format: yaml
  label: Dust Apps API
  slug: dust-tt-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-apps-api-openapi.yml
- filename: dust-tt-conversations-api-openapi.yml
  format: yaml
  label: Dust Conversations API
  slug: dust-tt-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-conversations-api-openapi.yml
- filename: dust-tt-datasources-api-openapi.yml
  format: yaml
  label: Dust Datasources API
  slug: dust-tt-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-datasources-api-openapi.yml
- filename: dust-tt-datasourceviews-api-openapi.yml
  format: yaml
  label: Dust DatasourceViews API
  slug: dust-tt-datasourceviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-datasourceviews-api-openapi.yml
- filename: dust-tt-feedbacks-api-openapi.yml
  format: yaml
  label: Dust Feedbacks API
  slug: dust-tt-feedbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-feedbacks-api-openapi.yml
- filename: dust-tt-mcp-api-openapi.yml
  format: yaml
  label: Dust MCP API
  slug: dust-tt-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-mcp-api-openapi.yml
- filename: dust-tt-mentions-api-openapi.yml
  format: yaml
  label: Dust Mentions API
  slug: dust-tt-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-mentions-api-openapi.yml
- filename: dust-tt-search-api-openapi.yml
  format: yaml
  label: Dust Search API
  slug: dust-tt-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-search-api-openapi.yml
- filename: dust-tt-skills-api-openapi.yml
  format: yaml
  label: Dust Skills API
  slug: dust-tt-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-skills-api-openapi.yml
- filename: dust-tt-spaces-api-openapi.yml
  format: yaml
  label: Dust Spaces API
  slug: dust-tt-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-spaces-api-openapi.yml
- filename: dust-tt-tools-api-openapi.yml
  format: yaml
  label: Dust Tools API
  slug: dust-tt-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-tools-api-openapi.yml
- filename: dust-tt-triggers-api-openapi.yml
  format: yaml
  label: Dust Triggers API
  slug: dust-tt-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-triggers-api-openapi.yml
- filename: dust-tt-workspace-api-openapi.yml
  format: yaml
  label: Dust Workspace API
  slug: dust-tt-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dust Tt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dust
provider_slug: dust-tt
scheme_count: 1
schemes:
- description: Your DUST API key is a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dust-agents-api-openapi.yml
  - openapi/dust-apps-api-openapi.yml
  - openapi/dust-conversations-api-openapi.yml
  - openapi/dust-datasources-api-openapi.yml
  - openapi/dust-mcp-api-openapi.yml
  - openapi/dust-search-api-openapi.yml
  - openapi/dust-skills-api-openapi.yml
  - openapi/dust-triggers-api-openapi.yml
  - openapi/dust-workspace-api-openapi.yml
  type: http
slug: dust-tt-authentication
source_filename: dust-tt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dust-agents-api-openapi.yml, openapi/dust-apps-api-openapi.yml, openapi/dust-conversations-api-openapi.yml,\n  openapi/dust-datasources-api-openapi.yml, openapi/dust-mcp-api-openapi.yml, openapi/dust-search-api-openapi.yml,\n  openapi/dust-skills-api-openapi.yml, openapi/dust-triggers-api-openapi.yml, openapi/dust-workspace-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Your DUST API key is a Bearer token.\n  sources:\n  - openapi/dust-agents-api-openapi.yml\n  - openapi/dust-apps-api-openapi.yml\n  - openapi/dust-conversations-api-openapi.yml\n  - openapi/dust-datasources-api-openapi.yml\n  - openapi/dust-mcp-api-openapi.yml\n  - openapi/dust-search-api-openapi.yml\n  - openapi/dust-skills-api-openapi.yml\n  - openapi/dust-triggers-api-openapi.yml\n  - openapi/dust-workspace-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/authentication/dust-tt-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- AI
- Artificial Intelligence
- Custom Workflows
- Data Sources
- Dust
- Enterprise AI
- Knowledge Management
- LLM
- MCP
- Multi-Model
- RAG
---
