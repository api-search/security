---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meetkuro-com-account-api-openapi.yml
  format: yaml
  label: Kuro Account API
  slug: meetkuro-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-account-api-openapi.yml
- filename: meetkuro-com-generations-api-openapi.yml
  format: yaml
  label: Kuro Generations API
  slug: meetkuro-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-generations-api-openapi.yml
- filename: meetkuro-com-models-api-openapi.yml
  format: yaml
  label: Kuro Models API
  slug: meetkuro-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-models-api-openapi.yml
- filename: meetkuro-com-recipes-api-openapi.yml
  format: yaml
  label: Kuro Recipes API
  slug: meetkuro-com-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-recipes-api-openapi.yml
- filename: meetkuro-com-runs-api-openapi.yml
  format: yaml
  label: Kuro Runs API
  slug: meetkuro-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-runs-api-openapi.yml
- filename: meetkuro-com-subjects-api-openapi.yml
  format: yaml
  label: Kuro Subjects API
  slug: meetkuro-com-subjects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-subjects-api-openapi.yml
- filename: meetkuro-com-uploads-api-openapi.yml
  format: yaml
  label: Kuro Uploads API
  slug: meetkuro-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meetkuro-com/openapi/meetkuro-com-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kuro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kuro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kuro
provider_slug: meetkuro-com
scheme_count: 1
schemes:
- description: A personal token (`KR_…`) from Settings → Connections.
  name: token
  scheme: bearer
  sources:
  - openapi/meetkuro-com-openapi.json
  type: http
slug: meetkuro-com-authentication
source_filename: meetkuro-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meetkuro-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: A personal token (`KR_…`) from Settings → Connections.\n  sources:\n  - openapi/meetkuro-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/meetkuro-com/authentication/meetkuro-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Media
- Content Creation
- Platform
- Software-as-a-Service
---
