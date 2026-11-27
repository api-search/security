---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eureka-md-openapi-generated.yml
  format: yaml
  label: Eureka Health API
  slug: eureka-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eureka-md/openapi/_ae-authored/eureka-md-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Eureka Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eureka Health declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Eureka Health
provider_slug: eureka-md
scheme_count: 1
schemes:
- description: Bearer token with per-doctor API key (eur_...)
  in: header
  name: Authorization
  type: apiKey
slug: eureka-md-authentication
source_filename: eureka-md-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://eureka.md/docs/mcp.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token with per-doctor API key (eur_...)\n"
source_yaml_url: https://artifacts.apis.io/eureka-md/authentication/eureka-md-authentication.yml
summary_line: 1 scheme
tags:
- Healthcare
- Automation
- Claims
- Prior Authorization
- Software-as-a-Service
---
