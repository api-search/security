---
api_key_in: []
api_specs:
- filename: render-com-openapi.yml
  format: yaml
  label: Render Services API
  slug: render-com-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Deploys API
  slug: render-com-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Custom Domains API
  slug: render-com-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Environment Variables & Secret Files API
  slug: render-com-env-vars-secret-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Environment Groups API
  slug: render-com-env-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Postgres API
  slug: render-com-postgres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Key Value API
  slug: render-com-key-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Jobs API
  slug: render-com-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Disks API
  slug: render-com-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Blueprints API
  slug: render-com-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Projects & Environments API
  slug: render-com-projects-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Workspaces & Members API
  slug: render-com-workspaces-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Metrics API
  slug: render-com-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Logs API
  slug: render-com-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Webhooks API
  slug: render-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Render Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Render secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Render
provider_slug: render-com
scheme_count: 1
schemes:
- description: Render API key created in the Render Dashboard, sent as an Authorization Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/render-com-openapi.yml
  type: http
slug: render-com-authentication
source_filename: render-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/render-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Render API key created in the Render Dashboard, sent as an Authorization Bearer\n    token.\n  sources:\n  - openapi/render-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/authentication/render-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Hosting
- PaaS
- Deployment
- Web Services
- Databases
- DevOps
---
