---
api_key_in: []
api_specs:
- filename: nutrientsdb-foods-api-openapi.yml
  format: yaml
  label: NutrientsDB Foods API
  slug: nutrientsdb-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrientsdb/refs/heads/main/openapi/nutrientsdb-foods-api-openapi.yml
auth_types: []
description: 'The NutrientsDB Sample API requires NO authentication. This is an explicit, documented posture, not an omission: the docs page states "No authentication" alongside "HTTPS" and "CORS enabled", and the OpenAPI declares no components.securitySchemes and no security requirement on its single operation. Verified by an anonymous live call that returned 200 with data. There are no API keys to issue, no OAuth surface, no scopes, and therefore no scopes/ artifact for this provider.'
kind: authentication
layout: security
method: searched
name: Nutrientsdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: NutrientsDB declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: NutrientsDB
provider_slug: nutrientsdb
scheme_count: 0
schemes: []
slug: nutrientsdb-authentication
source_filename: nutrientsdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://www.nutrientsdb.com/api/docs\nspec_source: openapi/nutrientsdb-sample-api-openapi.yml\ndocs: https://www.nutrientsdb.com/api/docs\ndescription: >-\n  The NutrientsDB Sample API requires NO authentication. This is an explicit, documented posture,\n  not an omission: the docs page states \"No authentication\" alongside \"HTTPS\" and \"CORS enabled\",\n  and the OpenAPI declares no components.securitySchemes and no security requirement on its single\n  operation. Verified by an anonymous live call that returned 200 with data. There are no API keys\n  to issue, no OAuth surface, no scopes, and therefore no scopes/ artifact for this provider.\nsummary:\n  types: []\n  authentication_required: false\n  anonymous_access: true\n  api_key_in: []\n  oauth2_flows: []\nschemes: []\npublic_access:\n  model: open-keyless-read-only\n  transport: https\n  methods_allowed: [GET, HEAD, OPTIONS]\n  cors:\n    enabled: true\n    access_control_allow_origin:\
  \ '*'\n    access_control_allow_methods: GET, HEAD, OPTIONS\n    access_control_allow_headers: Content-Type\n    notes: >-\n      Wildcard CORS with no credentials makes the endpoint directly callable from browser and agent\n      runtimes with no proxy or key-broker in front of it.\n  scope_of_access: >-\n    The keyless endpoint exposes only the public 1,000-food sample. The full ~2.9M-food NutrientsDB\n    dataset is not behind an authentication wall on this API — it is not exposed by this API at all.\n    It is sold as a one-time-license downloadable dataset for local use, so the commercial boundary\n    is a delivery boundary, not an auth boundary.\nx-evidence:\n  fetched: '2026-08-09'\n  probes:\n    - url: https://www.nutrientsdb.com/api/foods?q=banana&limit=2\n      http_status: 200\n      note: Anonymous request with no Authorization header or key parameter returned data.\n    - url: https://www.nutrientsdb.com/api/openapi\n      http_status: 200\n      note: OpenAPI 3.1.0 declares\
  \ no components.securitySchemes and no security[].\n    - url: https://www.nutrientsdb.com/api/docs\n      http_status: 200\n      note: Docs page states \"No authentication\".\ncross_links:\n  conventions: conventions/nutrientsdb-conventions.yml\n  conformance: conformance/nutrientsdb-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrientsdb/refs/heads/main/authentication/nutrientsdb-authentication.yml
summary_line: 0 schemes
tags:
- nutrition
- food
- nutrients
- food-composition
- data
- search
- sample-data
- dataset
- ai-builders
- reference-data
- open-data
- keyless-api
---
