---
api_key_in: []
api_specs:
- filename: rely-automations-api-openapi.yml
  format: yaml
  label: Rely.io Automations API
  slug: rely-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-automations-api-openapi.yml
- filename: rely-blueprints-api-openapi.yml
  format: yaml
  label: Rely.io Blueprints API
  slug: rely-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-blueprints-api-openapi.yml
- filename: rely-entities-api-openapi.yml
  format: yaml
  label: Rely.io Entities API
  slug: rely-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-entities-api-openapi.yml
- filename: rely-scorecards-api-openapi.yml
  format: yaml
  label: Rely.io Scorecards API
  slug: rely-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-scorecards-api-openapi.yml
- filename: rely-self-service-actions-api-openapi.yml
  format: yaml
  label: Rely.io Self-Service Actions API
  slug: rely-self-service-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-self-service-actions-api-openapi.yml
- filename: rely-users-api-openapi.yml
  format: yaml
  label: Rely.io Users API
  slug: rely-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/openapi/rely-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rely.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rely.io
provider_slug: rely
scheme_count: 1
schemes:
- description: Long-lived API key generated in the Rely.io Plugins settings page. Valid for 10 years. Include as Bearer token in Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rely-openapi.yml
  type: http
slug: rely-authentication
source_filename: rely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rely-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Long-lived API key generated in the Rely.io Plugins settings page. Valid for\n    10 years. Include as Bearer token in Authorization header.\n  sources:\n  - openapi/rely-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/authentication/rely-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Experience
- Internal Developer Portal
- Platform Engineering
- Software Catalog
- Service Catalog
- Engineering Scorecards
---
