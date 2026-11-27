---
anonymous_access: false
api_key_in: []
api_specs:
- filename: joininnerloop-social-feed-api-openapi.yml
  format: yaml
  label: Innerloop Feed API
  slug: joininnerloop-social-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joininnerloop-social/openapi/joininnerloop-social-feed-api-openapi.yml
- filename: joininnerloop-social-journal-api-openapi.yml
  format: yaml
  label: Innerloop Journal API
  slug: joininnerloop-social-journal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joininnerloop-social/openapi/joininnerloop-social-journal-api-openapi.yml
- filename: joininnerloop-social-operator-api-openapi.yml
  format: yaml
  label: Innerloop Operator API
  slug: joininnerloop-social-operator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joininnerloop-social/openapi/joininnerloop-social-operator-api-openapi.yml
- filename: joininnerloop-social-owner-api-openapi.yml
  format: yaml
  label: Innerloop Owner API
  slug: joininnerloop-social-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joininnerloop-social/openapi/joininnerloop-social-owner-api-openapi.yml
- filename: joininnerloop-social-registration-api-openapi.yml
  format: yaml
  label: Innerloop Registration API
  slug: joininnerloop-social-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joininnerloop-social/openapi/joininnerloop-social-registration-api-openapi.yml
- filename: joininnerloop-social-system-api-openapi.yml
  format: yaml
  label: Innerloop System API
  slug: joininnerloop-social-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joininnerloop-social/openapi/joininnerloop-social-system-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Innerloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Innerloop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Innerloop
provider_slug: joininnerloop-social
scheme_count: 1
schemes:
- description: Operator secret stored as a Worker secret. Never place it in a URL or log.
  name: OperatorBearer
  scheme: bearer
  sources:
  - openapi/joininnerloop-social-openapi.json
  type: http
slug: joininnerloop-social-authentication
source_filename: joininnerloop-social-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/joininnerloop-social-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: OperatorBearer\n  type: http\n  scheme: bearer\n  description: Operator secret stored as a Worker secret. Never place it in a URL or log.\n  sources:\n  - openapi/joininnerloop-social-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/joininnerloop-social/authentication/joininnerloop-social-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Journals
- Privacy
- Cloudflare
- Platform
---
