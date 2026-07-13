---
api_key_in: []
api_specs:
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Ports and Vessels API
  slug: sinay-ports-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Metocean API
  slug: sinay-metocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay CO2 Emission API
  slug: sinay-co2-emission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay ETA API
  slug: sinay-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Port Congestion API
  slug: sinay-port-congestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sinay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sinay secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sinay
provider_slug: sinay
scheme_count: 1
schemes:
- description: 'Every Sinay API endpoint requires authentication with an API key. The key is sent in a request header named API_KEY (for example `API_KEY: your-api-key`). The same scheme applies across all Sinay products (Ports & Vessels, Metocean, CO2 Emission, ETA, Port Congestion). Create a free key on the Sinay Developers Platform at https://developers.sinay.ai/. Confirmed from the live per-product Swagger securitySchemes (apiKey / header / API_KEY) on 2026-07-12.'
  in: header
  keyName: API_KEY
  name: ApiKey
  sources:
  - openapi/sinay-openapi.yml
  - https://api.sinay.ai/co2/api/v2/swagger.yaml
  - https://developers.sinay.ai/
  type: apiKey
slug: sinay-authentication
source_filename: sinay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/sinay-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  keyName: API_KEY\n  description: >-\n    Every Sinay API endpoint requires authentication with an API key. The key is\n    sent in a request header named API_KEY (for example `API_KEY: your-api-key`).\n    The same scheme applies across all Sinay products (Ports & Vessels, Metocean,\n    CO2 Emission, ETA, Port Congestion). Create a free key on the Sinay Developers\n    Platform at https://developers.sinay.ai/. Confirmed from the live per-product\n    Swagger securitySchemes (apiKey / header / API_KEY) on 2026-07-12.\n  sources:\n  - openapi/sinay-openapi.yml\n  - https://api.sinay.ai/co2/api/v2/swagger.yaml\n  - https://developers.sinay.ai/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/authentication/sinay-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vessel Tracking
- AIS
- Maritime
- Maritime Data
- Weather
- CO2 Emissions
- Port Congestion
- Ship Tracking
- ETA
- Ocean Data
---
