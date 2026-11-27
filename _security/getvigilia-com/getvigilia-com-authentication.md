---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getvigilia-com-account-api-openapi.yml
  format: yaml
  label: Vigilia Account API
  slug: getvigilia-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-account-api-openapi.yml
- filename: getvigilia-com-apps-api-openapi.yml
  format: yaml
  label: Vigilia Apps API
  slug: getvigilia-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-apps-api-openapi.yml
- filename: getvigilia-com-errors-api-openapi.yml
  format: yaml
  label: Vigilia Errors API
  slug: getvigilia-com-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-errors-api-openapi.yml
- filename: getvigilia-com-incidents-api-openapi.yml
  format: yaml
  label: Vigilia Incidents API
  slug: getvigilia-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-incidents-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Vigilia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vigilia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vigilia
provider_slug: getvigilia-com
scheme_count: 1
schemes:
- description: A personal access token (`vgs_…`) from Settings → API tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/getvigilia-com-openapi.json
  type: http
slug: getvigilia-com-authentication
source_filename: getvigilia-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getvigilia-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A personal access token (`vgs_…`) from Settings → API tokens.\n  sources:\n  - openapi/getvigilia-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getvigilia-com/authentication/getvigilia-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Monitoring
- DevOps
- Observability
- Company
---
