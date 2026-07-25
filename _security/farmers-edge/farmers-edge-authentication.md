---
api_key_in:
- query
api_specs:
- filename: farmers-edge-canplug-api-openapi.yml
  format: yaml
  label: Farmers Edge canplug API
  slug: farmers-edge-canplug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-canplug-api-openapi.yml
- filename: farmers-edge-carbon-api-openapi.yml
  format: yaml
  label: Farmers Edge carbon API
  slug: farmers-edge-carbon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-carbon-api-openapi.yml
- filename: farmers-edge-client-api-openapi.yml
  format: yaml
  label: Farmers Edge client API
  slug: farmers-edge-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-client-api-openapi.yml
- filename: farmers-edge-contact-api-openapi.yml
  format: yaml
  label: Farmers Edge contact API
  slug: farmers-edge-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-contact-api-openapi.yml
- filename: farmers-edge-gridcalc-api-openapi.yml
  format: yaml
  label: Farmers Edge gridcalc API
  slug: farmers-edge-gridcalc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-gridcalc-api-openapi.yml
- filename: farmers-edge-hefty-api-openapi.yml
  format: yaml
  label: Farmers Edge hefty API
  slug: farmers-edge-hefty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-hefty-api-openapi.yml
- filename: farmers-edge-integrations-api-openapi.yml
  format: yaml
  label: Farmers Edge integrations API
  slug: farmers-edge-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-integrations-api-openapi.yml
- filename: farmers-edge-labcommand-api-openapi.yml
  format: yaml
  label: Farmers Edge labcommand API
  slug: farmers-edge-labcommand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-labcommand-api-openapi.yml
- filename: farmers-edge-payments-api-openapi.yml
  format: yaml
  label: Farmers Edge payments API
  slug: farmers-edge-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-payments-api-openapi.yml
- filename: farmers-edge-recengine-api-openapi.yml
  format: yaml
  label: Farmers Edge recengine API
  slug: farmers-edge-recengine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-recengine-api-openapi.yml
- filename: farmers-edge-token-login-api-openapi.yml
  format: yaml
  label: Farmers Edge token-login API
  slug: farmers-edge-token-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-token-login-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Farmers Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farmers Edge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Farmers Edge
provider_slug: farmers-edge
scheme_count: 1
schemes:
- in: query
  name: FarmCommand Token
  parameter: token
  sources:
  - openapi/farmers-edge-farmcommand-openapi-original.json
  type: apiKey
slug: farmers-edge-authentication
source_filename: farmers-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/farmers-edge-farmcommand-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: FarmCommand Token\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/farmers-edge-farmcommand-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/authentication/farmers-edge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Agriculture
- Precision Agriculture
- AgTech
- Farm Management
- Digital Agriculture
- IoT
- Weather
- Carbon
- API
---
