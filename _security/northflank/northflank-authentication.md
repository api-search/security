---
api_key_in: []
api_specs:
- filename: northflank-addons-api-openapi.yml
  format: yaml
  label: Northflank Addons API
  slug: northflank-addons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/openapi/northflank-addons-api-openapi.yml
- filename: northflank-jobs-api-openapi.yml
  format: yaml
  label: Northflank Jobs API
  slug: northflank-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/openapi/northflank-jobs-api-openapi.yml
- filename: northflank-projects-api-openapi.yml
  format: yaml
  label: Northflank Projects API
  slug: northflank-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/openapi/northflank-projects-api-openapi.yml
- filename: northflank-services-api-openapi.yml
  format: yaml
  label: Northflank Services API
  slug: northflank-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/openapi/northflank-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Northflank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Northflank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Northflank
provider_slug: northflank
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/northflank-openapi.yml
  type: http
slug: northflank-authentication
source_filename: northflank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/northflank-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/northflank-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/authentication/northflank-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Deployment
- Developer Experience
- Internal Developer Platform
- Platform Engineering
---
