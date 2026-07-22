---
api_key_in:
- env/config
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pantomath Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pantomath secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pantomath
provider_slug: pantomath
scheme_count: 1
schemes:
- description: API key supplied to the Pantomath SDK (apiKey constructor option / the PANTOMATH_API_KEY environment variable) and sent against the tenant's PANTOMATH_API_BASE_URL ingestion endpoint.
  in: config
  name: apiKey
  parameter: PANTOMATH_API_KEY
  sources:
  - https://registry.npmjs.org/@pantomath/sdk-javascript
  type: apiKey
slug: pantomath-authentication
source_filename: pantomath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://registry.npmjs.org/@pantomath/sdk-javascript\ndocs: https://www.npmjs.com/package/@pantomath/sdk-javascript\nnotes: >-\n  Pantomath does not publish a public OpenAPI definition or developer\n  documentation portal (docs./api./developer. subdomains do not resolve), so this\n  profile is derived from the published first-party JavaScript SDK rather than a\n  machine-readable spec. The SDK configures the ingestion API with a base URL and\n  an API key (environment variables PANTOMATH_API_BASE_URL and PANTOMATH_API_KEY;\n  SDK constructor accepts { apiKey }), indicating API-key authentication over a\n  per-tenant base URL.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - env/config\nschemes:\n- name: apiKey\n  type: apiKey\n  in: config\n  parameter: PANTOMATH_API_KEY\n  description: >-\n    API key supplied to the Pantomath SDK (apiKey constructor option / the\n    PANTOMATH_API_KEY environment variable) and sent against\
  \ the tenant's\n    PANTOMATH_API_BASE_URL ingestion endpoint.\n  sources:\n  - https://registry.npmjs.org/@pantomath/sdk-javascript\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pantomath/refs/heads/main/authentication/pantomath-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Observability
- Data Operations
- Data Pipeline Monitoring
- Data Lineage
- Data Quality
- Data Reliability
- Analytics
---
