---
anonymous_access: false
api_key_in: []
api_specs:
- filename: autonet-work-utils-api-openapi.yml
  format: yaml
  label: Autonet Utils API
  slug: autonet-work-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autonet-work/openapi/autonet-work-utils-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Autonet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autonet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Autonet
provider_slug: autonet-work
scheme_count: 1
schemes:
- description: Provision via POST /api/v1/keys or Architect login
  in: header
  name: X-Autonet-Token
  type: apiKey
slug: autonet-work-authentication
source_filename: autonet-work-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: https://autonet.work/openapi.json\nschemes:\n  - type: apiKey\n    name: X-Autonet-Token\n    in: header\n    description: Provision via POST /api/v1/keys or Architect login"
source_yaml_url: https://artifacts.apis.io/autonet-work/authentication/autonet-work-authentication.yml
summary_line: 1 scheme
tags:
- Internet
- Utilities
- Agents
- Monitoring
---
