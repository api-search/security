---
api_key_in: []
api_specs:
- filename: daytona-sandbox-api-openapi.yml
  format: yaml
  label: Daytona Sandbox API
  slug: daytona-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-sandbox-api-openapi.yml
- filename: daytona-sandbox-toolbox-api-openapi.yml
  format: yaml
  label: Daytona Sandbox Toolbox API
  slug: daytona-sandbox-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-sandbox-toolbox-api-openapi.yml
- filename: daytona-snapshots-api-openapi.yml
  format: yaml
  label: Daytona Snapshots API
  slug: daytona-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-snapshots-api-openapi.yml
- filename: daytona-volumes-api-openapi.yml
  format: yaml
  label: Daytona Volumes API
  slug: daytona-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-volumes-api-openapi.yml
- filename: daytona-preview-api-openapi.yml
  format: yaml
  label: Daytona Preview API
  slug: daytona-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-preview-api-openapi.yml
- filename: daytona-webhooks-api-openapi.yml
  format: yaml
  label: Daytona Webhooks API
  slug: daytona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-webhooks-api-openapi.yml
- filename: daytona-organizations-api-openapi.yml
  format: yaml
  label: Daytona Organizations API
  slug: daytona-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-organizations-api-openapi.yml
- filename: daytona-api-keys-api-openapi.yml
  format: yaml
  label: Daytona API Keys API
  slug: daytona-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-api-keys-api-openapi.yml
- filename: daytona-users-api-openapi.yml
  format: yaml
  label: Daytona Users API
  slug: daytona-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-users-api-openapi.yml
- filename: daytona-admin-api-openapi.yml
  format: yaml
  label: Daytona Admin API
  slug: daytona-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-admin-api-openapi.yml
- filename: daytona-health-api-openapi.yml
  format: yaml
  label: Daytona Health API
  slug: daytona-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-health-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Daytona Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daytona secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Daytona
provider_slug: daytona-io
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: API Key access
  name: bearer
  scheme: bearer
  sources:
  - openapi/daytona-admin-api-openapi.yml
  - openapi/daytona-api-keys-api-openapi.yml
  - openapi/daytona-health-api-openapi.yml
  - openapi/daytona-organizations-api-openapi.yml
  - openapi/daytona-preview-api-openapi.yml
  - openapi/daytona-sandbox-api-openapi.yml
  - openapi/daytona-snapshots-api-openapi.yml
  - openapi/daytona-toolbox-api-openapi.yml
  - openapi/daytona-users-api-openapi.yml
  - openapi/daytona-volumes-api-openapi.yml
  - openapi/daytona-webhooks-api-openapi.yml
  type: http
- name: oauth2
  openIdConnectUrl: http://localhost:3000/.well-known/openid-configuration
  sources:
  - openapi/daytona-admin-api-openapi.yml
  - openapi/daytona-api-keys-api-openapi.yml
  - openapi/daytona-health-api-openapi.yml
  - openapi/daytona-organizations-api-openapi.yml
  - openapi/daytona-preview-api-openapi.yml
  - openapi/daytona-sandbox-api-openapi.yml
  - openapi/daytona-snapshots-api-openapi.yml
  - openapi/daytona-toolbox-api-openapi.yml
  - openapi/daytona-users-api-openapi.yml
  - openapi/daytona-volumes-api-openapi.yml
  - openapi/daytona-webhooks-api-openapi.yml
  type: openIdConnect
slug: daytona-io-authentication
source_filename: daytona-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/daytona-admin-api-openapi.yml, openapi/daytona-api-keys-api-openapi.yml, openapi/daytona-health-api-openapi.yml,\n  openapi/daytona-organizations-api-openapi.yml, openapi/daytona-preview-api-openapi.yml, openapi/daytona-sandbox-api-openapi.yml,\n  openapi/daytona-snapshots-api-openapi.yml, openapi/daytona-toolbox-api-openapi.yml, openapi/daytona-users-api-openapi.yml,\n  openapi/daytona-volumes-api-openapi.yml, openapi/daytona-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: API Key access\n  sources:\n  - openapi/daytona-admin-api-openapi.yml\n  - openapi/daytona-api-keys-api-openapi.yml\n  - openapi/daytona-health-api-openapi.yml\n  - openapi/daytona-organizations-api-openapi.yml\n  - openapi/daytona-preview-api-openapi.yml\n  - openapi/daytona-sandbox-api-openapi.yml\n  - openapi/daytona-snapshots-api-openapi.yml\n\
  \  - openapi/daytona-toolbox-api-openapi.yml\n  - openapi/daytona-users-api-openapi.yml\n  - openapi/daytona-volumes-api-openapi.yml\n  - openapi/daytona-webhooks-api-openapi.yml\n- name: oauth2\n  type: openIdConnect\n  openIdConnectUrl: http://localhost:3000/.well-known/openid-configuration\n  sources:\n  - openapi/daytona-admin-api-openapi.yml\n  - openapi/daytona-api-keys-api-openapi.yml\n  - openapi/daytona-health-api-openapi.yml\n  - openapi/daytona-organizations-api-openapi.yml\n  - openapi/daytona-preview-api-openapi.yml\n  - openapi/daytona-sandbox-api-openapi.yml\n  - openapi/daytona-snapshots-api-openapi.yml\n  - openapi/daytona-toolbox-api-openapi.yml\n  - openapi/daytona-users-api-openapi.yml\n  - openapi/daytona-volumes-api-openapi.yml\n  - openapi/daytona-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/authentication/daytona-io-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- AI
- Agents
- Artificial Intelligence
- Cloud
- Code Execution
- Computer Use
- Developer Tools
- Infrastructure
- Open Source
- Sandbox
- Secure Execution
---
