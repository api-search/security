---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myrmigo-com-agent-api-openapi.yml
  format: yaml
  label: Myrmigo Agent API
  slug: myrmigo-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myrmigo-com/openapi/myrmigo-com-agent-api-openapi.yml
- filename: myrmigo-com-healthz-api-openapi.yml
  format: yaml
  label: Myrmigo Healthz API
  slug: myrmigo-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myrmigo-com/openapi/myrmigo-com-healthz-api-openapi.yml
- filename: myrmigo-com-owner-api-openapi.yml
  format: yaml
  label: Myrmigo Owner API
  slug: myrmigo-com-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myrmigo-com/openapi/myrmigo-com-owner-api-openapi.yml
- filename: myrmigo-com-reference-api-openapi.yml
  format: yaml
  label: Myrmigo Reference API
  slug: myrmigo-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myrmigo-com/openapi/myrmigo-com-reference-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Myrmigo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Myrmigo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Myrmigo
provider_slug: myrmigo-com
scheme_count: 1
schemes:
- description: An mrm_live_ organisation key, issued by Myrmigo (not self-serve).
  name: bearer
  scheme: bearer
  sources:
  - openapi/myrmigo-com-openapi.json
  - openapi/openapi.json
  type: http
slug: myrmigo-com-authentication
source_filename: myrmigo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myrmigo-com-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: An mrm_live_ organisation key, issued by Myrmigo (not self-serve).\n  sources:\n  - openapi/myrmigo-com-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myrmigo-com/authentication/myrmigo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Automation
- PrivateBeta
- Navigation
- Platform
---
