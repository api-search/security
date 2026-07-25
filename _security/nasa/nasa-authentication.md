---
api_key_in:
- query
api_specs:
- filename: nasa-asset-api-openapi.yml
  format: yaml
  label: NASA Asset API
  slug: nasa-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-asset-api-openapi.yml
- filename: nasa-captions-api-openapi.yml
  format: yaml
  label: NASA Captions API
  slug: nasa-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-captions-api-openapi.yml
- filename: nasa-donki-api-openapi.yml
  format: yaml
  label: NASA DONKI API
  slug: nasa-donki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-donki-api-openapi.yml
- filename: nasa-epic-api-openapi.yml
  format: yaml
  label: NASA EPIC API
  slug: nasa-epic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-epic-api-openapi.yml
- filename: nasa-mars-photos-api-openapi.yml
  format: yaml
  label: NASA Mars Photos API
  slug: nasa-mars-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-mars-photos-api-openapi.yml
- filename: nasa-metadata-api-openapi.yml
  format: yaml
  label: NASA Metadata API
  slug: nasa-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-metadata-api-openapi.yml
- filename: nasa-neo-api-openapi.yml
  format: yaml
  label: NASA Neo API
  slug: nasa-neo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-neo-api-openapi.yml
- filename: nasa-planetary-api-openapi.yml
  format: yaml
  label: NASA Planetary API
  slug: nasa-planetary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-planetary-api-openapi.yml
- filename: nasa-search-api-openapi.yml
  format: yaml
  label: NASA Search API
  slug: nasa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nasa Authentication
name_suffix: Authentication
oauth_flows: []
overview: NASA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NASA
provider_slug: nasa
scheme_count: 1
schemes:
- demo_key: DEMO_KEY
  in: query
  name: api_key
  parameter: api_key
  signup: https://api.nasa.gov/
  sources:
  - openapi/nasa-apod-openapi.yml
  - openapi/nasa-donki-openapi.yml
  - openapi/nasa-epic-openapi.yml
  - openapi/nasa-mars-rover-photos-openapi.yml
  - openapi/nasa-neo-openapi.yml
  type: apiKey
slug: nasa-authentication
source_filename: nasa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/*.yml (api_key query parameter) + https://api.nasa.gov/ auth docs\ndocs: https://api.nasa.gov/\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nnotes: >-\n  Every NASA Open API is authenticated with a single api_key query parameter on\n  api.nasa.gov (and images-api.nasa.gov for the Image and Video Library, whose\n  read endpoints are open). The specs model api_key as a required query parameter\n  rather than a formal OpenAPI securityScheme, so mechanical derivation finds no\n  scheme; this profile is authored from the parameter + published docs. There is\n  no OAuth, OIDC, mTLS, or scope surface. DEMO_KEY is a shared public key for\n  exploration (see sandbox/). Higher rate limits require emailing api@nasa.gov.\nschemes:\n  - name: api_key\n    type: apiKey\n    in: query\n    parameter: api_key\n    sources:\n      - openapi/nasa-apod-openapi.yml\n      - openapi/nasa-donki-openapi.yml\n  \
  \    - openapi/nasa-epic-openapi.yml\n      - openapi/nasa-mars-rover-photos-openapi.yml\n      - openapi/nasa-neo-openapi.yml\n    demo_key: DEMO_KEY\n    signup: https://api.nasa.gov/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/authentication/nasa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Science
- Space
---
