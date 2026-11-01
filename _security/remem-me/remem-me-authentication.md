---
anonymous_access: false
api_key_in: []
api_specs:
- filename: remem-me-access-api-openapi.yml
  format: yaml
  label: remem-me Access API
  slug: remem-me-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/remem-me/openapi/remem-me-access-api-openapi.yml
- filename: remem-me-collections-api-openapi.yml
  format: yaml
  label: remem-me Collections API
  slug: remem-me-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/remem-me/openapi/remem-me-collections-api-openapi.yml
- filename: remem-me-replication-api-openapi.yml
  format: yaml
  label: remem-me Replication API
  slug: remem-me-replication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/remem-me/openapi/remem-me-replication-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Remem Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: remem-me declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: remem-me
provider_slug: remem-me
scheme_count: 2
schemes:
- description: Session cookie for web authentication
  in: cookie
  name: sessionid
  type: apiKey
- bearerFormat: JWT
  description: JWT Bearer token authentication
  scheme: bearer
  type: http
slug: remem-me-authentication
source_filename: remem-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://rpl.remem.me/api/docs.json\nschemes:\n  - type: apiKey\n    in: cookie\n    name: sessionid\n    description: Session cookie for web authentication\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: JWT Bearer token authentication\n"
source_yaml_url: https://artifacts.apis.io/remem-me/authentication/remem-me-authentication.yml
summary_line: 2 schemes
tags:
- Bible
- Memory
- Nonprofit
- Education
- MobileApp
- OpenSource
---
