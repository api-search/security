---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: parkypass-com-live-api-openapi.yml
  format: yaml
  label: Parky Live API
  slug: parkypass-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-live-api-openapi.yml
- filename: parkypass-com-meta-api-openapi.yml
  format: yaml
  label: Parky Meta API
  slug: parkypass-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-meta-api-openapi.yml
- filename: parkypass-com-parks-api-openapi.yml
  format: yaml
  label: Parky Parks API
  slug: parkypass-com-parks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-parks-api-openapi.yml
- filename: parkypass-com-resorts-api-openapi.yml
  format: yaml
  label: Parky Resorts API
  slug: parkypass-com-resorts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-resorts-api-openapi.yml
- filename: parkypass-com-rides-api-openapi.yml
  format: yaml
  label: Parky Rides API
  slug: parkypass-com-rides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parkypass-com/openapi/parkypass-com-rides-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Parky Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parky secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Parky
provider_slug: parkypass-com
scheme_count: 3
schemes:
- bearerFormat: pk_live_ followed by 32 letters and digits
  description: 'Optional developer key: `Authorization: Bearer pk_live_...`. Get one at https://parkypass.com/developers.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parkypass-com-openapi.json
  type: http
- description: Optional developer key in a header, for clients that cannot set Authorization.
  in: header
  name: parkyKeyHeader
  parameter: X-Parky-Key
  sources:
  - openapi/parkypass-com-openapi.json
  type: apiKey
- description: Streams only (EventSource and browser WebSockets cannot set headers).
  in: query
  name: parkyKeyQuery
  parameter: key
  sources:
  - openapi/parkypass-com-openapi.json
  type: apiKey
slug: parkypass-com-authentication
source_filename: parkypass-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/parkypass-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: pk_live_ followed by 32 letters and digits\n  description: 'Optional developer key: `Authorization: Bearer pk_live_...`. Get one at https://parkypass.com/developers.'\n  sources:\n  - openapi/parkypass-com-openapi.json\n- name: parkyKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Parky-Key\n  description: Optional developer key in a header, for clients that cannot set Authorization.\n  sources:\n  - openapi/parkypass-com-openapi.json\n- name: parkyKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Streams only (EventSource and browser WebSockets cannot set headers).\n  sources:\n  - openapi/parkypass-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/parkypass-com/authentication/parkypass-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- ThemePark
- Mobile App
- Travel
- Disney
- Universal
---
