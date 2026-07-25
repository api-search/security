---
api_key_in: []
api_specs:
- filename: mlsgrid-lookup-api-openapi.yml
  format: yaml
  label: mlsgrid Lookup API
  slug: mlsgrid-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-lookup-api-openapi.yml
- filename: mlsgrid-media-api-openapi.yml
  format: yaml
  label: mlsgrid Media API
  slug: mlsgrid-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-media-api-openapi.yml
- filename: mlsgrid-member-api-openapi.yml
  format: yaml
  label: mlsgrid Member API
  slug: mlsgrid-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-member-api-openapi.yml
- filename: mlsgrid-metadata-api-openapi.yml
  format: yaml
  label: mlsgrid Metadata API
  slug: mlsgrid-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-metadata-api-openapi.yml
- filename: mlsgrid-office-api-openapi.yml
  format: yaml
  label: mlsgrid Office API
  slug: mlsgrid-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-office-api-openapi.yml
- filename: mlsgrid-openhouse-api-openapi.yml
  format: yaml
  label: mlsgrid OpenHouse API
  slug: mlsgrid-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-openhouse-api-openapi.yml
- filename: mlsgrid-property-api-openapi.yml
  format: yaml
  label: mlsgrid Property API
  slug: mlsgrid-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/openapi/mlsgrid-property-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mlsgrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: mlsgrid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mlsgrid
provider_slug: mlsgrid
scheme_count: 1
schemes:
- bearerFormat: OAuth2
  description: Long-lived OAuth 2.0 bearer token issued via the MLS Grid web application token tab.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mlsgrid-reso-web-api-openapi.yml
  type: http
slug: mlsgrid-authentication
source_filename: mlsgrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mlsgrid-reso-web-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: Long-lived OAuth 2.0 bearer token issued via the MLS Grid web application token\n    tab.\n  sources:\n  - openapi/mlsgrid-reso-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mlsgrid/refs/heads/main/authentication/mlsgrid-authentication.yml
summary_line: http · 1 scheme
tags: []
---
