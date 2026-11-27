---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: getlandlens-com-colleges-api-openapi.yml
  format: yaml
  label: LandLens Colleges API
  slug: getlandlens-com-colleges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlandlens-com/openapi/getlandlens-com-colleges-api-openapi.yml
- filename: getlandlens-com-landlords-api-openapi.yml
  format: yaml
  label: LandLens Landlords API
  slug: getlandlens-com-landlords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlandlens-com/openapi/getlandlens-com-landlords-api-openapi.yml
- filename: getlandlens-com-properties-api-openapi.yml
  format: yaml
  label: LandLens Properties API
  slug: getlandlens-com-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlandlens-com/openapi/getlandlens-com-properties-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LandLens Authentication
name_suffix: Authentication
oauth_flows: []
overview: LandLens secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LandLens
provider_slug: getlandlens-com
scheme_count: 1
schemes:
- description: Optional. Raises the quota to your plan. Get one at https://getlandlens.com/api
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/getlandlens-com-openapi.json
  type: apiKey
slug: getlandlens-com-authentication
source_filename: getlandlens-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getlandlens-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional. Raises the quota to your plan. Get one at https://getlandlens.com/api\n  sources:\n  - openapi/getlandlens-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getlandlens-com/authentication/getlandlens-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real Estate
- Student Housing
- Data Platform
- Reviews
---
