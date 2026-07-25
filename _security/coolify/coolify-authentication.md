---
api_key_in: []
api_specs:
- filename: coolify-applications-api-openapi.yml
  format: yaml
  label: Coolify Applications API
  slug: coolify-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-applications-api-openapi.yml
- filename: coolify-cloud-tokens-api-openapi.yml
  format: yaml
  label: Coolify Cloud Tokens API
  slug: coolify-cloud-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-cloud-tokens-api-openapi.yml
- filename: coolify-databases-api-openapi.yml
  format: yaml
  label: Coolify Databases API
  slug: coolify-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-databases-api-openapi.yml
- filename: coolify-deployments-api-openapi.yml
  format: yaml
  label: Coolify Deployments API
  slug: coolify-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-deployments-api-openapi.yml
- filename: coolify-disable-api-openapi.yml
  format: yaml
  label: Coolify Disable API
  slug: coolify-disable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-disable-api-openapi.yml
- filename: coolify-enable-api-openapi.yml
  format: yaml
  label: Coolify Enable API
  slug: coolify-enable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-enable-api-openapi.yml
- filename: coolify-github-apps-api-openapi.yml
  format: yaml
  label: Coolify GitHub Apps API
  slug: coolify-github-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-github-apps-api-openapi.yml
- filename: coolify-health-api-openapi.yml
  format: yaml
  label: Coolify Health API
  slug: coolify-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-health-api-openapi.yml
- filename: coolify-hetzner-api-openapi.yml
  format: yaml
  label: Coolify Hetzner API
  slug: coolify-hetzner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-hetzner-api-openapi.yml
- filename: coolify-mcp-api-openapi.yml
  format: yaml
  label: Coolify Mcp API
  slug: coolify-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-mcp-api-openapi.yml
- filename: coolify-private-keys-api-openapi.yml
  format: yaml
  label: Coolify Private Keys API
  slug: coolify-private-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-private-keys-api-openapi.yml
- filename: coolify-projects-api-openapi.yml
  format: yaml
  label: Coolify Projects API
  slug: coolify-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-projects-api-openapi.yml
- filename: coolify-resources-api-openapi.yml
  format: yaml
  label: Coolify Resources API
  slug: coolify-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-resources-api-openapi.yml
- filename: coolify-scheduled-tasks-api-openapi.yml
  format: yaml
  label: Coolify Scheduled Tasks API
  slug: coolify-scheduled-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-scheduled-tasks-api-openapi.yml
- filename: coolify-servers-api-openapi.yml
  format: yaml
  label: Coolify Servers API
  slug: coolify-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-servers-api-openapi.yml
- filename: coolify-services-api-openapi.yml
  format: yaml
  label: Coolify Services API
  slug: coolify-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-services-api-openapi.yml
- filename: coolify-teams-api-openapi.yml
  format: yaml
  label: Coolify Teams API
  slug: coolify-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-teams-api-openapi.yml
- filename: coolify-version-api-openapi.yml
  format: yaml
  label: Coolify Version API
  slug: coolify-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-version-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coolify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coolify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coolify
provider_slug: coolify
scheme_count: 1
schemes:
- description: Go to `Keys & Tokens` / `API tokens` and create a new token. Use the token as the bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coolify-openapi.yml
  type: http
slug: coolify-authentication
source_filename: coolify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coolify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Go to `Keys & Tokens` / `API tokens` and create a new token. Use the token as\n    the bearer token.\n  sources:\n  - openapi/coolify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/authentication/coolify-authentication.yml
summary_line: http · 1 scheme
tags:
- Platform as a Service
- Self-Hosting
- Deployment
- Open Source
- Containers
- Docker
---
