---
api_key_in:
- header
api_specs:
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Networks API
  slug: megaphone-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Podcasts API
  slug: megaphone-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Episodes API
  slug: megaphone-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Campaigns and Orders API
  slug: megaphone-campaigns-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Direct Sales API v2
  slug: megaphone-direct-sales-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Metrics and Impressions Export API
  slug: megaphone-metrics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Megaphone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Megaphone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Megaphone
provider_slug: megaphone
scheme_count: 1
schemes:
- description: 'Per-user API token sent as `Authorization: Token token="<API_TOKEN>"`. Generated on account creation and managed under User Settings; treat as a password and do not reuse across organizations.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/megaphone-openapi.yml
  type: apiKey
slug: megaphone-authentication
source_filename: megaphone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/megaphone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Per-user API token sent as `Authorization: Token token=\"<API_TOKEN>\"`. Generated\n    on account creation and managed under User Settings; treat as a password and do not reuse\n    across organizations.'\n  sources:\n  - openapi/megaphone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/authentication/megaphone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Advertising
- Ad Monetization
- Dynamic Ad Insertion
- Media
- Spotify
---
