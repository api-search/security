---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 3dvalley-com-account-api-openapi.yml
  format: yaml
  label: 3D Valley Account API
  slug: 3dvalley-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-account-api-openapi.yml
- filename: 3dvalley-com-assets-api-openapi.yml
  format: yaml
  label: 3D Valley Assets API
  slug: 3dvalley-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-assets-api-openapi.yml
- filename: 3dvalley-com-categories-api-openapi.yml
  format: yaml
  label: 3D Valley Categories API
  slug: 3dvalley-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-categories-api-openapi.yml
- filename: 3dvalley-com-jobs-api-openapi.yml
  format: yaml
  label: 3D Valley Jobs API
  slug: 3dvalley-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-jobs-api-openapi.yml
- filename: 3dvalley-com-tools-api-openapi.yml
  format: yaml
  label: 3D Valley Tools API
  slug: 3dvalley-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-tools-api-openapi.yml
- filename: 3dvalley-com-uploads-api-openapi.yml
  format: yaml
  label: 3D Valley Uploads API
  slug: 3dvalley-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 3D Valley Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3D Valley secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 3D Valley
provider_slug: 3dvalley-com
scheme_count: 1
schemes:
- description: An API key (3dv_live_...) or an OAuth access token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/3dvalley-com-openapi.json
  type: http
slug: 3dvalley-com-authentication
source_filename: 3dvalley-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/3dvalley-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: An API key (3dv_live_...) or an OAuth access token.\n  sources:\n  - openapi/3dvalley-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/3dvalley-com/authentication/3dvalley-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Generation
- Texture Generation
- Asset Library
- Browser Tools
---
