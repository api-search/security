---
anonymous_access: false
api_key_in: []
api_specs:
- filename: voltcast-com-prices-api-openapi.yml
  format: yaml
  label: voltcast-com Prices API
  slug: voltcast-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/voltcast-com/openapi/voltcast-com-prices-api-openapi.yml
- filename: voltcast-com-public-api-openapi.yml
  format: yaml
  label: voltcast-com Public API
  slug: voltcast-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/voltcast-com/openapi/voltcast-com-public-api-openapi.yml
- filename: voltcast-com-zones-api-openapi.yml
  format: yaml
  label: voltcast-com Zones API
  slug: voltcast-com-zones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/voltcast-com/openapi/voltcast-com-zones-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Voltcast Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: voltcast-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: voltcast-com
provider_slug: voltcast-com
scheme_count: 1
schemes:
- description: API key from https://voltcast.com/dashboard
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/voltcast-com-openapi.json
  type: http
slug: voltcast-com-authentication
source_filename: voltcast-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/voltcast-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from https://voltcast.com/dashboard\n  sources:\n  - openapi/voltcast-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/voltcast-com/authentication/voltcast-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Media
- Platform
---
