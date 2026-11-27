---
anonymous_access: false
api_key_in: []
api_specs:
- filename: taktovka-com-absences-api-openapi.yml
  format: yaml
  label: Taktovka Absences API
  slug: taktovka-com-absences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-absences-api-openapi.yml
- filename: taktovka-com-attendance-api-openapi.yml
  format: yaml
  label: Taktovka Attendance API
  slug: taktovka-com-attendance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-attendance-api-openapi.yml
- filename: taktovka-com-company-api-openapi.yml
  format: yaml
  label: Taktovka Company API
  slug: taktovka-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-company-api-openapi.yml
- filename: taktovka-com-meta-api-openapi.yml
  format: yaml
  label: Taktovka Meta API
  slug: taktovka-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-meta-api-openapi.yml
- filename: taktovka-com-people-api-openapi.yml
  format: yaml
  label: Taktovka People API
  slug: taktovka-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-people-api-openapi.yml
- filename: taktovka-com-schedules-api-openapi.yml
  format: yaml
  label: Taktovka Schedules API
  slug: taktovka-com-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-schedules-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Taktovka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taktovka secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taktovka
provider_slug: taktovka-com
scheme_count: 1
schemes:
- description: A company key, tk_ followed by 43 characters
  name: bearer
  scheme: bearer
  sources:
  - openapi/taktovka-com-openapi.json
  type: http
slug: taktovka-com-authentication
source_filename: taktovka-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/taktovka-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A company key, tk_ followed by 43 characters\n  sources:\n  - openapi/taktovka-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/taktovka-com/authentication/taktovka-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
