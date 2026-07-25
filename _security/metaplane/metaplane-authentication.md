---
api_key_in:
- header
api_specs:
- filename: metaplane-connections-api-openapi.yml
  format: yaml
  label: Metaplane Connections API
  slug: metaplane-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-connections-api-openapi.yml
- filename: metaplane-datapoints-api-openapi.yml
  format: yaml
  label: Metaplane Datapoints API
  slug: metaplane-datapoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-datapoints-api-openapi.yml
- filename: metaplane-monitors-api-openapi.yml
  format: yaml
  label: Metaplane Monitors API
  slug: metaplane-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-monitors-api-openapi.yml
- filename: metaplane-tags-api-openapi.yml
  format: yaml
  label: Metaplane Tags API
  slug: metaplane-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/openapi/metaplane-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metaplane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metaplane secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Metaplane
provider_slug: metaplane
scheme_count: 1
schemes:
- description: Metaplane API key
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/metaplane-openapi.yml
  type: apiKey
slug: metaplane-authentication
source_filename: metaplane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metaplane-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Metaplane API key\n  sources:\n  - openapi/metaplane-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metaplane/refs/heads/main/authentication/metaplane-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AIOps
- Data Observability
---
