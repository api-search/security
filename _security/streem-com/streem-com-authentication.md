---
anonymous_access: false
api_key_in: []
api_specs:
- filename: streem-com-companies-api-openapi.yml
  format: yaml
  label: Greply Companies API
  slug: streem-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/streem-com/openapi/streem-com-companies-api-openapi.yml
- filename: streem-com-groups-api-openapi.yml
  format: yaml
  label: Greply Groups API
  slug: streem-com-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/streem-com/openapi/streem-com-groups-api-openapi.yml
- filename: streem-com-images-api-openapi.yml
  format: yaml
  label: Greply Images API
  slug: streem-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/streem-com/openapi/streem-com-images-api-openapi.yml
- filename: streem-com-rooms-api-openapi.yml
  format: yaml
  label: Greply Rooms API
  slug: streem-com-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/streem-com/openapi/streem-com-rooms-api-openapi.yml
- filename: streem-com-users-api-openapi.yml
  format: yaml
  label: Greply Users API
  slug: streem-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/streem-com/openapi/streem-com-users-api-openapi.yml
- filename: streem-com-webhooks-api-openapi.yml
  format: yaml
  label: Greply Webhooks API
  slug: streem-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/streem-com/openapi/streem-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Streem Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greply secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Greply
provider_slug: streem-com
scheme_count: 2
schemes:
- name: api-key
  scheme: basic
  sources:
  - openapi/streem-com-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: bearer-auth
  scheme: bearer
  sources:
  - openapi/streem-com-api-openapi.yml
  type: http
slug: streem-com-authentication
source_filename: streem-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: derived\nsource: openapi/streem-com-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api-key\n  type: http\n  scheme: basic\n  sources:\n  - openapi/streem-com-api-openapi.yml\n- name: bearer-auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/streem-com-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/streem-com/authentication/streem-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Data Analytics
- Real-time
- API Platform
- Streaming
---
