---
api_key_in: []
api_specs:
- filename: scalable-platforms-artifacts-api-openapi.yml
  format: yaml
  label: Scalable Platforms Artifacts API
  slug: scalable-platforms-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-artifacts-api-openapi.yml
- filename: scalable-platforms-deployments-api-openapi.yml
  format: yaml
  label: Scalable Platforms Deployments API
  slug: scalable-platforms-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-deployments-api-openapi.yml
- filename: scalable-platforms-domains-api-openapi.yml
  format: yaml
  label: Scalable Platforms Domains API
  slug: scalable-platforms-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-domains-api-openapi.yml
- filename: scalable-platforms-environments-api-openapi.yml
  format: yaml
  label: Scalable Platforms Environments API
  slug: scalable-platforms-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-environments-api-openapi.yml
- filename: scalable-platforms-projects-api-openapi.yml
  format: yaml
  label: Scalable Platforms Projects API
  slug: scalable-platforms-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-projects-api-openapi.yml
- filename: scalable-platforms-teams-api-openapi.yml
  format: yaml
  label: Scalable Platforms Teams API
  slug: scalable-platforms-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Platforms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Platforms secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Platforms
provider_slug: scalable-platforms
scheme_count: 1
schemes:
- bearerFormat: VercelToken
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/scalable-platforms-openapi.yml
  type: http
slug: scalable-platforms-authentication
source_filename: scalable-platforms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-platforms-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: VercelToken\n  sources:\n  - openapi/scalable-platforms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/authentication/scalable-platforms-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
---
