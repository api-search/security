---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: bee-maps-account-api-openapi.yml
  format: yaml
  label: Bee Maps Account API
  slug: bee-maps-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-account-api-openapi.yml
- filename: bee-maps-ai-events-api-openapi.yml
  format: yaml
  label: Bee Maps AI Events API
  slug: bee-maps-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-ai-events-api-openapi.yml
- filename: bee-maps-bursts-api-openapi.yml
  format: yaml
  label: Bee Maps Bursts API
  slug: bee-maps-bursts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-bursts-api-openapi.yml
- filename: bee-maps-devices-api-openapi.yml
  format: yaml
  label: Bee Maps Devices API
  slug: bee-maps-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-devices-api-openapi.yml
- filename: bee-maps-imagery-api-openapi.yml
  format: yaml
  label: Bee Maps Imagery API
  slug: bee-maps-imagery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-imagery-api-openapi.yml
- filename: bee-maps-map-features-api-openapi.yml
  format: yaml
  label: Bee Maps Map Features API
  slug: bee-maps-map-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-map-features-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bee Maps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bee Maps secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bee Maps
provider_slug: bee-maps
scheme_count: 2
schemes:
- description: 'API key passed as Basic auth header: `Authorization: Basic <API_KEY>`'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/openapi.json
  type: http
- description: API key passed as query parameter (used for burst endpoints)
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/openapi.json
  type: apiKey
slug: bee-maps-authentication
source_filename: bee-maps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: 'API key passed as Basic auth header: `Authorization: Basic <API_KEY>`'\n  sources:\n  - openapi/openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key passed as query parameter (used for burst endpoints)\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/authentication/bee-maps-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Mapping
- GIS
- Location
- Data
---
