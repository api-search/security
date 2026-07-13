---
api_key_in: []
api_specs:
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Metrics Export API
  slug: metrics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Deployments & Events Ingestion API
  slug: deployments-events-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Investment Categories API
  slug: investment-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Webhooks & Notifications API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Swarmia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swarmia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swarmia
provider_slug: swarmia
scheme_count: 1
schemes:
- description: Bearer API token provisioned at https://app.swarmia.com/settings/api-tokens. Built-in/custom reports require the entityQuery scope; AI usage ingestion requires the aiUsage scope. GET endpoints also accept the token via a ?token= query parameter.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/swarmia-openapi.yml
  type: http
slug: swarmia-authentication
source_filename: swarmia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swarmia-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: Bearer API token provisioned at https://app.swarmia.com/settings/api-tokens.\n    Built-in/custom reports require the entityQuery scope; AI usage ingestion requires the aiUsage\n    scope. GET endpoints also accept the token via a ?token= query parameter.\n  sources:\n  - openapi/swarmia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/authentication/swarmia-authentication.yml
summary_line: http · 1 scheme
tags:
- Engineering Effectiveness
- Developer Productivity
- DORA
- Software Delivery
- Analytics
---
