---
api_key_in:
- header
api_specs:
- filename: treblle-analytics-api-openapi.yml
  format: yaml
  label: Treblle Analytics API
  slug: treblle-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-analytics-api-openapi.yml
- filename: treblle-endpoints-api-openapi.yml
  format: yaml
  label: Treblle Endpoints API
  slug: treblle-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-endpoints-api-openapi.yml
- filename: treblle-governance-api-openapi.yml
  format: yaml
  label: Treblle Governance API
  slug: treblle-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-governance-api-openapi.yml
- filename: treblle-members-api-openapi.yml
  format: yaml
  label: Treblle Members API
  slug: treblle-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-members-api-openapi.yml
- filename: treblle-projects-api-openapi.yml
  format: yaml
  label: Treblle Projects API
  slug: treblle-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-projects-api-openapi.yml
- filename: treblle-requests-api-openapi.yml
  format: yaml
  label: Treblle Requests API
  slug: treblle-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-requests-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Treblle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Treblle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Treblle
provider_slug: treblle
scheme_count: 1
schemes:
- description: Treblle API key obtained from the Treblle workspace settings. Pass the API key in the Treblle-Api-Key header.
  in: header
  name: apiKeyAuth
  parameter: Treblle-Api-Key
  sources:
  - openapi/treblle-api-openapi.yml
  type: apiKey
slug: treblle-authentication
source_filename: treblle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/treblle-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Treblle-Api-Key\n  description: Treblle API key obtained from the Treblle workspace settings. Pass the API key\n    in the Treblle-Api-Key header.\n  sources:\n  - openapi/treblle-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/authentication/treblle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Artificial Intelligence
- Developer Experience
- Documentation
- Governance
- Insights
- Observability
- Platform
- Security
- Testing
---
