---
api_key_in:
- header
api_specs:
- filename: fulcrum-audio-api-openapi.yml
  format: yaml
  label: Fulcrum Audio API
  slug: fulcrum-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-audio-api-openapi.yml
- filename: fulcrum-changesets-api-openapi.yml
  format: yaml
  label: Fulcrum Changesets API
  slug: fulcrum-changesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-changesets-api-openapi.yml
- filename: fulcrum-choice-lists-api-openapi.yml
  format: yaml
  label: Fulcrum Choice Lists API
  slug: fulcrum-choice-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-choice-lists-api-openapi.yml
- filename: fulcrum-classification-sets-api-openapi.yml
  format: yaml
  label: Fulcrum Classification Sets API
  slug: fulcrum-classification-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-classification-sets-api-openapi.yml
- filename: fulcrum-forms-api-openapi.yml
  format: yaml
  label: Fulcrum Forms API
  slug: fulcrum-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-forms-api-openapi.yml
- filename: fulcrum-layers-api-openapi.yml
  format: yaml
  label: Fulcrum Layers API
  slug: fulcrum-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-layers-api-openapi.yml
- filename: fulcrum-memberships-api-openapi.yml
  format: yaml
  label: Fulcrum Memberships API
  slug: fulcrum-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-memberships-api-openapi.yml
- filename: fulcrum-photos-api-openapi.yml
  format: yaml
  label: Fulcrum Photos API
  slug: fulcrum-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-photos-api-openapi.yml
- filename: fulcrum-projects-api-openapi.yml
  format: yaml
  label: Fulcrum Projects API
  slug: fulcrum-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-projects-api-openapi.yml
- filename: fulcrum-query-api-openapi.yml
  format: yaml
  label: Fulcrum Query API
  slug: fulcrum-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-query-api-openapi.yml
- filename: fulcrum-records-api-openapi.yml
  format: yaml
  label: Fulcrum Records API
  slug: fulcrum-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-records-api-openapi.yml
- filename: fulcrum-roles-api-openapi.yml
  format: yaml
  label: Fulcrum Roles API
  slug: fulcrum-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-roles-api-openapi.yml
- filename: fulcrum-signatures-api-openapi.yml
  format: yaml
  label: Fulcrum Signatures API
  slug: fulcrum-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-signatures-api-openapi.yml
- filename: fulcrum-videos-api-openapi.yml
  format: yaml
  label: Fulcrum Videos API
  slug: fulcrum-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-videos-api-openapi.yml
- filename: fulcrum-webhooks-api-openapi.yml
  format: yaml
  label: Fulcrum Webhooks API
  slug: fulcrum-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/openapi/fulcrum-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fulcrum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fulcrum secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fulcrum
provider_slug: fulcrum
scheme_count: 1
schemes:
- description: Fulcrum API token issued from a Fulcrum account
  in: header
  name: ApiToken
  parameter: X-ApiToken
  sources:
  - openapi/fulcrum-api-openapi.yml
  type: apiKey
slug: fulcrum-authentication
source_filename: fulcrum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fulcrum-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-ApiToken\n  description: Fulcrum API token issued from a Fulcrum account\n  sources:\n  - openapi/fulcrum-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulcrum/refs/heads/main/authentication/fulcrum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Collection
- Field Data
- Geospatial
- Process Management
- Mobile
---
