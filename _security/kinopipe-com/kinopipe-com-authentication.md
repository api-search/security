---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kinopipe-com-jobs-api-openapi.yml
  format: yaml
  label: KinoPipe Jobs API
  slug: kinopipe-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinopipe-com/openapi/kinopipe-com-jobs-api-openapi.yml
- filename: kinopipe-com-tools-api-openapi.yml
  format: yaml
  label: KinoPipe Tools API
  slug: kinopipe-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinopipe-com/openapi/kinopipe-com-tools-api-openapi.yml
- filename: kinopipe-com-uploads-api-openapi.yml
  format: yaml
  label: KinoPipe Uploads API
  slug: kinopipe-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinopipe-com/openapi/kinopipe-com-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: KinoPipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: KinoPipe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KinoPipe
provider_slug: kinopipe-com
scheme_count: 1
schemes:
- description: A KinoPipe API key beginning with kp_live_.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kinopipe-com-openapi.json
  type: http
slug: kinopipe-com-authentication
source_filename: kinopipe-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kinopipe-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A KinoPipe API key beginning with kp_live_.\n  sources:\n  - openapi/kinopipe-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kinopipe-com/authentication/kinopipe-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Editing
- Artificial Intelligence
- REST API
- MCP
- Open Source
- Company
---
