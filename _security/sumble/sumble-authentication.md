---
api_key_in: []
api_specs:
- filename: sumble-contact-lists-api-openapi.yml
  format: yaml
  label: Sumble contact-lists API
  slug: sumble-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-contact-lists-api-openapi.yml
- filename: sumble-jobs-api-openapi.yml
  format: yaml
  label: Sumble jobs API
  slug: sumble-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-jobs-api-openapi.yml
- filename: sumble-organization-lists-api-openapi.yml
  format: yaml
  label: Sumble organization-lists API
  slug: sumble-organization-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organization-lists-api-openapi.yml
- filename: sumble-organizations-api-openapi.yml
  format: yaml
  label: Sumble organizations API
  slug: sumble-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organizations-api-openapi.yml
- filename: sumble-people-api-openapi.yml
  format: yaml
  label: Sumble people API
  slug: sumble-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-people-api-openapi.yml
- filename: sumble-projects-api-openapi.yml
  format: yaml
  label: Sumble projects API
  slug: sumble-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-projects-api-openapi.yml
- filename: sumble-signals-api-openapi.yml
  format: yaml
  label: Sumble signals API
  slug: sumble-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-signals-api-openapi.yml
- filename: sumble-support-api-openapi.yml
  format: yaml
  label: Sumble support API
  slug: sumble-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-support-api-openapi.yml
- filename: sumble-teams-api-openapi.yml
  format: yaml
  label: Sumble teams API
  slug: sumble-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-teams-api-openapi.yml
- filename: sumble-technologies-api-openapi.yml
  format: yaml
  label: Sumble technologies API
  slug: sumble-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-technologies-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sumble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sumble secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sumble
provider_slug: sumble
scheme_count: 1
schemes:
- name: api_token
  scheme: bearer
  sources:
  - openapi/sumble-openapi-original.json
  type: http
slug: sumble-authentication
source_filename: sumble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sumble-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: api_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sumble-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/authentication/sumble-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Account Intelligence
- Sales Intelligence
- Data Enrichment
- Go-To-Market
- Technographics
- People Data
- Job Posts
- Signals
- MCP
---
