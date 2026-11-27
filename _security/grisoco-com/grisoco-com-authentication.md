---
anonymous_access: false
api_key_in: []
api_specs:
- filename: grisoco-com-check-api-openapi.yml
  format: yaml
  label: Grisoco AI Check API
  slug: grisoco-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grisoco-com/openapi/grisoco-com-check-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Grisoco AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grisoco AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grisoco AI
provider_slug: grisoco-com
scheme_count: 1
schemes:
- description: A Grisoco API key (grisoco_sk_…), created at https://grisoco.com/app under Create API key. The same key used for audits.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/grisoco-com-openapi.json
  type: http
slug: grisoco-com-authentication
source_filename: grisoco-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/grisoco-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: A Grisoco API key (grisoco_sk_…), created at https://grisoco.com/app under Create\n    API key. The same key used for audits.\n  sources:\n  - openapi/grisoco-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/grisoco-com/authentication/grisoco-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Smart-contract
- Artificial Intelligence
- Security
- Audit
- Payments
---
