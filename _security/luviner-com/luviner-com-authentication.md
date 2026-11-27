---
anonymous_access: false
api_key_in: []
api_specs:
- filename: luviner-com-account-api-openapi.yml
  format: yaml
  label: Luviner Account API
  slug: luviner-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-account-api-openapi.yml
- filename: luviner-com-catalog-api-openapi.yml
  format: yaml
  label: Luviner Catalog API
  slug: luviner-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-catalog-api-openapi.yml
- filename: luviner-com-inference-api-openapi.yml
  format: yaml
  label: Luviner Inference API
  slug: luviner-com-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-inference-api-openapi.yml
- filename: luviner-com-models-api-openapi.yml
  format: yaml
  label: Luviner Models API
  slug: luviner-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-models-api-openapi.yml
- filename: luviner-com-synthetic-data-api-openapi.yml
  format: yaml
  label: Luviner Synthetic Data API
  slug: luviner-com-synthetic-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-synthetic-data-api-openapi.yml
- filename: luviner-com-training-api-openapi.yml
  format: yaml
  label: Luviner Training API
  slug: luviner-com-training-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-training-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Luviner Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luviner secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Luviner
provider_slug: luviner-com
scheme_count: 1
schemes:
- description: API token from your Luviner dashboard (Settings > API Access)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/luviner-com-openapi.json
  type: http
slug: luviner-com-authentication
source_filename: luviner-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/luviner-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API token from your Luviner dashboard (Settings > API Access)\n  sources:\n  - openapi/luviner-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/luviner-com/authentication/luviner-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Bot Protection
- Self-Hosted
- Web Security
- Italy
---
