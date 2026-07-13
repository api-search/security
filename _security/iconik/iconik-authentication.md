---
api_key_in:
- header
api_specs:
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Assets API
  slug: iconik-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Collections API
  slug: iconik-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Metadata API
  slug: iconik-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Search API
  slug: iconik-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Files API
  slug: iconik-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
- filename: iconik-openapi.yml
  format: yaml
  label: iconik Jobs API
  slug: iconik-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/openapi/iconik-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Iconik Authentication
name_suffix: Authentication
oauth_flows: []
overview: iconik secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: iconik
provider_slug: iconik
scheme_count: 2
schemes:
- description: The iconik application ID generated in the web UI.
  in: header
  name: appId
  parameter: App-ID
  sources:
  - openapi/iconik-openapi.yml
  type: apiKey
- description: The iconik auth token paired with the application ID.
  in: header
  name: authToken
  parameter: Auth-Token
  sources:
  - openapi/iconik-openapi.yml
  type: apiKey
slug: iconik-authentication
source_filename: iconik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iconik-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appId\n  type: apiKey\n  in: header\n  parameter: App-ID\n  description: The iconik application ID generated in the web UI.\n  sources:\n  - openapi/iconik-openapi.yml\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: Auth-Token\n  description: The iconik auth token paired with the application ID.\n  sources:\n  - openapi/iconik-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iconik/refs/heads/main/authentication/iconik-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Media Asset Management
- MAM
- Video
- Media
- Cloud Storage
- Metadata
- Search
- Assets
---
