---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: billboardbug-com-ai-api-openapi.yml
  format: yaml
  label: BillboardBug AI API
  slug: billboardbug-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-ai-api-openapi.yml
- filename: billboardbug-com-blob-api-openapi.yml
  format: yaml
  label: BillboardBug Blob API
  slug: billboardbug-com-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-blob-api-openapi.yml
- filename: billboardbug-com-business-api-openapi.yml
  format: yaml
  label: BillboardBug Business API
  slug: billboardbug-com-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-business-api-openapi.yml
- filename: billboardbug-com-globalconfig-api-openapi.yml
  format: yaml
  label: BillboardBug Global Config API
  slug: billboardbug-com-globalconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-globalconfig-api-openapi.yml
- filename: billboardbug-com-post-api-openapi.yml
  format: yaml
  label: BillboardBug Post API
  slug: billboardbug-com-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-post-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BillboardBug Authentication
name_suffix: Authentication
oauth_flows: []
overview: BillboardBug secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BillboardBug
provider_slug: billboardbug-com
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/billboardbug-com-openapi.json
  type: apiKey
slug: billboardbug-com-authentication
source_filename: billboardbug-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/billboardbug-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/billboardbug-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/billboardbug-com/authentication/billboardbug-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Advertising
- Local Business
- Mobile App
- Small Business
---
