---
anonymous_access: false
api_key_in: []
api_specs:
- filename: imagefactory-co-kr-external-api-openapi.yml
  format: yaml
  label: Imagefactory External API
  slug: imagefactory-co-kr-external-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagefactory-co-kr/openapi/imagefactory-co-kr-external-api-openapi.yml
- filename: imagefactory-co-kr-generate-api-openapi.yml
  format: yaml
  label: Imagefactory Generate API
  slug: imagefactory-co-kr-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagefactory-co-kr/openapi/imagefactory-co-kr-generate-api-openapi.yml
- filename: imagefactory-co-kr-reports-api-openapi.yml
  format: yaml
  label: Imagefactory Reports API
  slug: imagefactory-co-kr-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagefactory-co-kr/openapi/imagefactory-co-kr-reports-api-openapi.yml
- filename: imagefactory-co-kr-resize-api-openapi.yml
  format: yaml
  label: Imagefactory Resize API
  slug: imagefactory-co-kr-resize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagefactory-co-kr/openapi/imagefactory-co-kr-resize-api-openapi.yml
- filename: imagefactory-co-kr-tasks-api-openapi.yml
  format: yaml
  label: Imagefactory Tasks API
  slug: imagefactory-co-kr-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagefactory-co-kr/openapi/imagefactory-co-kr-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Imagefactory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imagefactory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Imagefactory
provider_slug: imagefactory-co-kr
scheme_count: 1
schemes:
- bearerFormat: imf_<token>:<secret>
  description: API keys are issued from the Imagefactory account dashboard (My Page → API Keys). Team owners and admins can issue integration keys with usage:read permission.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/imagefactory-co-kr-openapi.json
  type: http
slug: imagefactory-co-kr-authentication
source_filename: imagefactory-co-kr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/imagefactory-co-kr-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: imf_<token>:<secret>\n  description: API keys are issued from the Imagefactory account dashboard (My Page → API Keys).\n    Team owners and admins can issue integration keys with usage:read permission.\n  sources:\n  - openapi/imagefactory-co-kr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/imagefactory-co-kr/authentication/imagefactory-co-kr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
