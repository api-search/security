---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vectorpanda-com-collections-api-openapi.yml
  format: yaml
  label: vectorpanda-com Collections API
  slug: vectorpanda-com-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vectorpanda-com/openapi/vectorpanda-com-collections-api-openapi.yml
- filename: vectorpanda-com-health-api-openapi.yml
  format: yaml
  label: vectorpanda-com Health API
  slug: vectorpanda-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vectorpanda-com/openapi/vectorpanda-com-health-api-openapi.yml
- filename: vectorpanda-com-query-api-openapi.yml
  format: yaml
  label: vectorpanda-com Query API
  slug: vectorpanda-com-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vectorpanda-com/openapi/vectorpanda-com-query-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Vectorpanda Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: vectorpanda-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: vectorpanda-com
provider_slug: vectorpanda-com
scheme_count: 1
schemes:
- description: 'API key issued from the dashboard. Pass as `Authorization: Bearer <api_key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vectorpanda-com-openapi.yml
  type: http
slug: vectorpanda-com-authentication
source_filename: vectorpanda-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/vectorpanda-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued from the dashboard. Pass as `Authorization: Bearer <api_key>`.'\n  sources:\n  - openapi/vectorpanda-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/vectorpanda-com/authentication/vectorpanda-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Vector Database
- Semantic Search
- Embeddings
---
