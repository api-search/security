---
api_key_in:
- query
- body
api_specs:
- filename: shipfinder-ais-data-api-ais-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API AIS Dataset API
  slug: shipfinder-ais-data-api-ais-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-ais-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-china-coastline-warning-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API China Coastline Warning Dataset API
  slug: shipfinder-ais-data-api-china-coastline-warning-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-china-coastline-warning-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-event-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Event Dataset API
  slug: shipfinder-ais-data-api-event-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-event-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-history-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API History Dataset API
  slug: shipfinder-ais-data-api-history-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-history-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-meteorology-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Meteorology Dataset API
  slug: shipfinder-ais-data-api-meteorology-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-meteorology-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-prediction-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Prediction Dataset API
  slug: shipfinder-ais-data-api-prediction-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-prediction-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-voyage-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Voyage Dataset API
  slug: shipfinder-ais-data-api-voyage-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-voyage-dataset-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shipfinder Ais Data Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: ShipFinder AIS Data API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ShipFinder AIS Data API
provider_slug: shipfinder-ais-data-api
scheme_count: 1
schemes:
- description: Every GET operation carries the API key as the "key" query parameter. The ten POST/DELETE Event-dataset operations accept the same key as a "key" property in the JSON request body. There is no bearer token, no OAuth 2.0 and no OIDC surface.
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/shipfinder-ais-data-api-openapi.yml
  type: apiKey
slug: shipfinder-ais-data-api-authentication
source_filename: shipfinder-ais-data-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/shipfinder-ais-data-api-openapi.yml\ndocs: https://docs.shipfinder.com/9177505m0\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - body\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/shipfinder-ais-data-api-openapi.yml\n  description: Every GET operation carries the API key as the \"key\" query parameter. The ten POST/DELETE Event-dataset\n    operations accept the same key as a \"key\" property in the JSON request body. There is no bearer token, no OAuth\n    2.0 and no OIDC surface.\nkey_management:\n  console: https://open.shipfinder.com/v1/console/overview\n  signup: https://www.shipfinder.com/home/register\n  tutorial: https://docs.shipfinder.com/9177505m0\n  key_types:\n  - name: Starter (Trial) Key\n    self_service: true\n    description: Preset permission scope\
  \ for evaluation and integration testing; usable immediately. One Starter\n      key per account.\n  - name: Custom (Production / Test) Key\n    self_service: false\n    description: Created with no active services. The ShipFinder business team confirms requirements by email and\n      enables the corresponding per-service permissions, normally within one business day.\n  max_keys_per_account: 5\n  domain_binding: Keys can be bound to a calling domain. A request from an unbound domain is rejected with envelope\n    status 14.\n  per_service_permissions: Datasets are individually permissioned. Calling a service the key is not entitled to\n    returns envelope status 21 (no service usage permission).\nnotes:\n- The key travels in the query string, so it appears in server logs, proxies and browser history; ShipFinder documents\n  no header-based alternative.\n- 'The marketing page at https://open.shipfinder.com/ shows an illustrative snippet using \"Authorization: Bearer\n  YOUR_API_KEY\"\
  \ against GET /v1/vessel/position. Neither the bearer scheme nor that path exists in the published\n  API documentation — treat the marketing snippet as illustrative.'\nx-evidence:\n- url: https://docs.shipfinder.com/9177505m0.md\n  http_status: 200\n  fetched: '2026-08-09'\n- url: https://open.shipfinder.com/\n  http_status: 200\n  fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/authentication/shipfinder-ais-data-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AIS
- Maritime Data
- Vessel Tracking
- Ship Tracking
- Vessel Data
- Historical AIS
- Geospatial
- GIS
- Logistics
- Supply Chain
- Weather
- Meteorology
- Trade
- Commodities
- Compliance
- Risk
- Event Streaming
- Webhooks
---
