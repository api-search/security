---
api_key_in:
- header
api_specs:
- filename: honeycomb-api-openapi.yml
  format: yaml
  label: Honeycomb API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-api-openapi.yml
- filename: honeycomb-events-api-openapi.yml
  format: yaml
  label: Honeycomb Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-events-api-openapi.yml
- filename: honeycomb-queries-api-openapi.yml
  format: yaml
  label: Honeycomb Queries API
  slug: queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-queries-api-openapi.yml
- filename: honeycomb-slos-api-openapi.yml
  format: yaml
  label: Honeycomb SLOs API
  slug: slos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-slos-api-openapi.yml
- filename: honeycomb-datasets-api-openapi.yml
  format: yaml
  label: Honeycomb Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-datasets-api-openapi.yml
- filename: honeycomb-boards-api-openapi.yml
  format: yaml
  label: Honeycomb Boards API
  slug: boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-boards-api-openapi.yml
- filename: honeycomb-markers-api-openapi.yml
  format: yaml
  label: Honeycomb Markers API
  slug: markers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-markers-api-openapi.yml
- filename: honeycomb-triggers-api-openapi.yml
  format: yaml
  label: Honeycomb Triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-triggers-api-openapi.yml
- filename: honeycomb-environments-api-openapi.yml
  format: yaml
  label: Honeycomb Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/openapi/honeycomb-environments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Honeycomb Authentication
name_suffix: Authentication
oauth_flows: []
overview: honeycomb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: honeycomb
provider_slug: honeycomb
scheme_count: 1
schemes:
- description: Honeycomb Configuration API key. Must have appropriate permissions for the endpoint being called.
  in: header
  name: ApiKeyAuth
  parameter: X-Honeycomb-Team
  sources:
  - openapi/honeycomb-api-openapi.yml
  - openapi/honeycomb-boards-api-openapi.yml
  - openapi/honeycomb-datasets-api-openapi.yml
  - openapi/honeycomb-environments-api-openapi.yml
  - openapi/honeycomb-events-api-openapi.yml
  - openapi/honeycomb-markers-api-openapi.yml
  - openapi/honeycomb-queries-api-openapi.yml
  - openapi/honeycomb-slos-api-openapi.yml
  - openapi/honeycomb-triggers-api-openapi.yml
  type: apiKey
slug: honeycomb-authentication
source_filename: honeycomb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/honeycomb-api-openapi.yml, openapi/honeycomb-boards-api-openapi.yml, openapi/honeycomb-datasets-api-openapi.yml,\n  openapi/honeycomb-environments-api-openapi.yml, openapi/honeycomb-events-api-openapi.yml,\n  openapi/honeycomb-markers-api-openapi.yml, openapi/honeycomb-queries-api-openapi.yml, openapi/honeycomb-slos-api-openapi.yml,\n  openapi/honeycomb-triggers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Honeycomb-Team\n  description: Honeycomb Configuration API key. Must have appropriate permissions for the endpoint\n    being called.\n  sources:\n  - openapi/honeycomb-api-openapi.yml\n  - openapi/honeycomb-boards-api-openapi.yml\n  - openapi/honeycomb-datasets-api-openapi.yml\n  - openapi/honeycomb-environments-api-openapi.yml\n  - openapi/honeycomb-events-api-openapi.yml\n  - openapi/honeycomb-markers-api-openapi.yml\n\
  \  - openapi/honeycomb-queries-api-openapi.yml\n  - openapi/honeycomb-slos-api-openapi.yml\n  - openapi/honeycomb-triggers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/authentication/honeycomb-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
