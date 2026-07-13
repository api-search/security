---
api_key_in:
- header
api_specs:
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Shows API
  slug: transistor-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Episodes API
  slug: transistor-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Analytics API
  slug: transistor-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Subscribers API
  slug: transistor-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
- filename: transistor-openapi.yml
  format: yaml
  label: Transistor Webhooks API
  slug: transistor-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/openapi/transistor-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Transistor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transistor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transistor
provider_slug: transistor
scheme_count: 1
schemes:
- description: API key generated in the Transistor dashboard Account area.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/transistor-openapi.yml
  type: apiKey
slug: transistor-authentication
source_filename: transistor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transistor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated in the Transistor dashboard Account area.\n  sources:\n  - openapi/transistor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transistor/refs/heads/main/authentication/transistor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Analytics
- Media
- Audio
- JSON:API
---
