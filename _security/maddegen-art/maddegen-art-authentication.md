---
anonymous_access: false
api_key_in: []
api_specs:
- filename: maddegen-art-pump-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Pump Cortex API
  slug: maddegen-art-pump-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-pump-cortex-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Maddegen Art Authentication
name_suffix: Authentication
oauth_flows: []
overview: maddegen-art declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: maddegen-art
provider_slug: maddegen-art
scheme_count: 1
schemes:
- description: Bearer hk_… prepaid credit key (POST /hub/api/v1/keys). Paid tools also accept it instead of x402.
  in: header
  name: Authorization
  type: apiKey
slug: maddegen-art-authentication
source_filename: maddegen-art-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: https://augur-trade.com/hub/openapi.json\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer hk_… prepaid credit key (POST /hub/api/v1/keys). Paid tools also accept it instead of x402.\n"
source_yaml_url: https://artifacts.apis.io/maddegen-art/authentication/maddegen-art-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
