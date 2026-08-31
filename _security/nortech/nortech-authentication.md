---
api_key_in: []
api_specs:
- filename: nortech-asset-api-openapi.yml
  format: yaml
  label: Nortech Asset API
  slug: nortech-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-asset-api-openapi.yml
- filename: nortech-deriver-api-openapi.yml
  format: yaml
  label: Nortech Deriver API
  slug: nortech-deriver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-deriver-api-openapi.yml
- filename: nortech-division-api-openapi.yml
  format: yaml
  label: Nortech Division API
  slug: nortech-division-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-division-api-openapi.yml
- filename: nortech-health-api-openapi.yml
  format: yaml
  label: Nortech Health API
  slug: nortech-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-health-api-openapi.yml
- filename: nortech-historical-data-api-openapi.yml
  format: yaml
  label: Nortech Historical Data API
  slug: nortech-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-historical-data-api-openapi.yml
- filename: nortech-import-data-api-openapi.yml
  format: yaml
  label: Nortech Import Data API
  slug: nortech-import-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-import-data-api-openapi.yml
- filename: nortech-live-data-api-openapi.yml
  format: yaml
  label: Nortech Live Data API
  slug: nortech-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-live-data-api-openapi.yml
- filename: nortech-me-api-openapi.yml
  format: yaml
  label: Nortech Me API
  slug: nortech-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-me-api-openapi.yml
- filename: nortech-mqtt-live-data-api-openapi.yml
  format: yaml
  label: Nortech MQTT Live Data API
  slug: nortech-mqtt-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-mqtt-live-data-api-openapi.yml
- filename: nortech-signal-api-openapi.yml
  format: yaml
  label: Nortech Signal API
  slug: nortech-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-signal-api-openapi.yml
- filename: nortech-unit-api-openapi.yml
  format: yaml
  label: Nortech Unit API
  slug: nortech-unit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-unit-api-openapi.yml
- filename: nortech-workspace-api-openapi.yml
  format: yaml
  label: Nortech Workspace API
  slug: nortech-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-workspace-api-openapi.yml
- filename: nortech-historicaldata-api-openapi.yml
  format: yaml
  label: Nortech Historical Data API
  slug: nortech-historicaldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/openapi/nortech-historicaldata-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nortech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nortech secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nortech
provider_slug: nortech
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: Bearer Token
  scheme: bearer
  sources:
  - openapi/nortech-openapi-original.json
  type: http
slug: nortech-authentication
source_filename: nortech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nortech-openapi-original.json\ndocs: https://docs.apps.nor.tech/cloud-apis-sdks-http-api\nnotes: >-\n  HTTP Bearer (JWT) authentication. Tokens are provisioned on request from\n  support@nortech.ai. The same Bearer token is used as the MQTT broker password\n  for live-data streaming.\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nortech-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nortech/refs/heads/main/authentication/nortech-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Industrial IoT
- IIoT
- Maritime
- Operational Data
- Time Series
- Sensors
- Data Infrastructure
---
