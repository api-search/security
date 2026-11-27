---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hlido-eu-directory-api-openapi.yml
  format: yaml
  label: Hlido Directory API
  slug: hlido-eu-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-directory-api-openapi.yml
- filename: hlido-eu-incidents-api-openapi.yml
  format: yaml
  label: Hlido Incidents API
  slug: hlido-eu-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-incidents-api-openapi.yml
- filename: hlido-eu-ops-api-openapi.yml
  format: yaml
  label: Hlido Ops API
  slug: hlido-eu-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-ops-api-openapi.yml
- filename: hlido-eu-recommendations-api-openapi.yml
  format: yaml
  label: Hlido Recommendations API
  slug: hlido-eu-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlido-eu/openapi/hlido-eu-recommendations-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hlido Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hlido secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hlido
provider_slug: hlido-eu
scheme_count: 1
schemes:
- bearerFormat: hlk_live
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hlido-eu-openapi.json
  type: http
slug: hlido-eu-authentication
source_filename: hlido-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hlido-eu-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: hlk_live\n  sources:\n  - openapi/hlido-eu-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hlido-eu/authentication/hlido-eu-authentication.yml
summary_line: http · 1 scheme
tags:
- Satellite
- Artificial Intelligence
- Earth Observation
- Czech
- Startups
---
