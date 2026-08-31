---
api_key_in: []
api_specs:
- filename: daytona-admin-api-openapi.yml
  format: yaml
  label: Daytona admin API
  slug: daytona-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-admin-api-openapi.yml
- filename: daytona-api-keys-api-openapi.yml
  format: yaml
  label: Daytona api-keys API
  slug: daytona-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-api-keys-api-openapi.yml
- filename: daytona-audit-api-openapi.yml
  format: yaml
  label: Daytona audit API
  slug: daytona-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-audit-api-openapi.yml
- filename: daytona-config-api-openapi.yml
  format: yaml
  label: Daytona config API
  slug: daytona-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-config-api-openapi.yml
- filename: daytona-docker-registry-api-openapi.yml
  format: yaml
  label: Daytona docker-registry API
  slug: daytona-docker-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-docker-registry-api-openapi.yml
- filename: daytona-health-api-openapi.yml
  format: yaml
  label: Daytona Health API
  slug: daytona-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-health-api-openapi.yml
- filename: daytona-jobs-api-openapi.yml
  format: yaml
  label: Daytona jobs API
  slug: daytona-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-jobs-api-openapi.yml
- filename: daytona-object-storage-api-openapi.yml
  format: yaml
  label: Daytona object-storage API
  slug: daytona-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-object-storage-api-openapi.yml
- filename: daytona-organizations-api-openapi.yml
  format: yaml
  label: Daytona organizations API
  slug: daytona-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-organizations-api-openapi.yml
- filename: daytona-preview-api-openapi.yml
  format: yaml
  label: Daytona preview API
  slug: daytona-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-preview-api-openapi.yml
- filename: daytona-regions-api-openapi.yml
  format: yaml
  label: Daytona regions API
  slug: daytona-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-regions-api-openapi.yml
- filename: daytona-runners-api-openapi.yml
  format: yaml
  label: Daytona runners API
  slug: daytona-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-runners-api-openapi.yml
- filename: daytona-sandbox-api-openapi.yml
  format: yaml
  label: Daytona sandbox API
  slug: daytona-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-sandbox-api-openapi.yml
- filename: daytona-snapshots-api-openapi.yml
  format: yaml
  label: Daytona snapshots API
  slug: daytona-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-snapshots-api-openapi.yml
- filename: daytona-toolbox-api-openapi.yml
  format: yaml
  label: Daytona toolbox API
  slug: daytona-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-toolbox-api-openapi.yml
- filename: daytona-users-api-openapi.yml
  format: yaml
  label: Daytona users API
  slug: daytona-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-users-api-openapi.yml
- filename: daytona-volumes-api-openapi.yml
  format: yaml
  label: Daytona volumes API
  slug: daytona-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-volumes-api-openapi.yml
- filename: daytona-webhooks-api-openapi.yml
  format: yaml
  label: Daytona webhooks API
  slug: daytona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-webhooks-api-openapi.yml
- filename: daytona-workspace-api-openapi.yml
  format: yaml
  label: Daytona workspace API
  slug: daytona-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-workspace-api-openapi.yml
- filename: daytona-daytona-api-openapi.yml
  format: yaml
  label: Daytona Daytona API
  slug: daytona-daytona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/openapi/daytona-daytona-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Daytona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daytona secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Daytona
provider_slug: daytona
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: API Key access
  name: bearer
  scheme: bearer
  sources:
  - openapi/daytona-openapi.json
  type: http
- name: oauth2
  openIdConnectUrl: http://localhost:3000/.well-known/openid-configuration
  sources:
  - openapi/daytona-openapi.json
  type: openIdConnect
slug: daytona-authentication
source_filename: daytona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/daytona-openapi.json\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: API Key access\n  sources:\n  - openapi/daytona-openapi.json\n- name: oauth2\n  type: openIdConnect\n  openIdConnectUrl: http://localhost:3000/.well-known/openid-configuration\n  sources:\n  - openapi/daytona-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daytona/refs/heads/main/authentication/daytona-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Sandboxes
- Secure Execution
- AI Agents
- Coding Agents
- Code Interpreter
- Snapshots
- Multi-Region
- HIPAA
- SOC 2
- GDPR
- Python
- TypeScript
- Open-Source
- LSP
---
