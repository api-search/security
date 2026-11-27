---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tenmomo-com-activate-api-openapi.yml
  format: yaml
  label: Tenmomo Activate API
  slug: tenmomo-com-activate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenmomo-com/openapi/tenmomo-com-activate-api-openapi.yml
- filename: tenmomo-com-categories-api-openapi.yml
  format: yaml
  label: Tenmomo Categories API
  slug: tenmomo-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenmomo-com/openapi/tenmomo-com-categories-api-openapi.yml
- filename: tenmomo-com-deals-api-openapi.yml
  format: yaml
  label: Tenmomo Deals API
  slug: tenmomo-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenmomo-com/openapi/tenmomo-com-deals-api-openapi.yml
- filename: tenmomo-com-stores-api-openapi.yml
  format: yaml
  label: Tenmomo Stores API
  slug: tenmomo-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenmomo-com/openapi/tenmomo-com-stores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tenmomo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tenmomo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tenmomo
provider_slug: tenmomo-com
scheme_count: 1
schemes:
- description: Tenmomo API key (sk-tm-...). Get one at https://tenmomo.com/dashboard#ai-credits
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tenmomo-com-openapi.json
  type: http
slug: tenmomo-com-authentication
source_filename: tenmomo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/tenmomo-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Tenmomo API key (sk-tm-...). Get one at https://tenmomo.com/dashboard#ai-credits\n  sources:\n  - openapi/tenmomo-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tenmomo-com/authentication/tenmomo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Coupon Codes
- Cashback
---
