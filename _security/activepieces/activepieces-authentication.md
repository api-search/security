---
api_key_in: []
api_specs:
- filename: activepieces-connections-api-openapi.yml
  format: yaml
  label: Activepieces Connections API
  slug: activepieces-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-connections-api-openapi.yml
- filename: activepieces-flow-runs-api-openapi.yml
  format: yaml
  label: Activepieces Flow Runs API
  slug: activepieces-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-flow-runs-api-openapi.yml
- filename: activepieces-flows-api-openapi.yml
  format: yaml
  label: Activepieces Flows API
  slug: activepieces-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-flows-api-openapi.yml
- filename: activepieces-folders-api-openapi.yml
  format: yaml
  label: Activepieces Folders API
  slug: activepieces-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-folders-api-openapi.yml
- filename: activepieces-pieces-api-openapi.yml
  format: yaml
  label: Activepieces Pieces API
  slug: activepieces-pieces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-pieces-api-openapi.yml
- filename: activepieces-projects-api-openapi.yml
  format: yaml
  label: Activepieces Projects API
  slug: activepieces-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-projects-api-openapi.yml
- filename: activepieces-templates-api-openapi.yml
  format: yaml
  label: Activepieces Templates API
  slug: activepieces-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-templates-api-openapi.yml
- filename: activepieces-users-api-openapi.yml
  format: yaml
  label: Activepieces Users API
  slug: activepieces-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-users-api-openapi.yml
- filename: activepieces-worker-machines-api-openapi.yml
  format: yaml
  label: Activepieces Worker Machines API
  slug: activepieces-worker-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces-worker-machines-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Activepieces Authentication
name_suffix: Authentication
oauth_flows: []
overview: Activepieces secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Activepieces
provider_slug: activepieces
scheme_count: 1
schemes:
- description: API key from the Activepieces admin console, passed as a Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/activepieces.json
  type: http
slug: activepieces-authentication
source_filename: activepieces-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activepieces.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key from the Activepieces admin console, passed as a Bearer token\n  sources:\n  - openapi/activepieces.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/authentication/activepieces-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- No-Code
- Open-Source
- Workflows
- AI Agents
- MCP
---
