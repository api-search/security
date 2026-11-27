---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fairvalid-com-balance-api-openapi.yml
  format: yaml
  label: FairValid Balance API
  slug: fairvalid-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-balance-api-openapi.yml
- filename: fairvalid-com-fairmatch-api-openapi.yml
  format: yaml
  label: FairValid Fair Match API
  slug: fairvalid-com-fairmatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-fairmatch-api-openapi.yml
- filename: fairvalid-com-jobs-api-openapi.yml
  format: yaml
  label: FairValid Jobs API
  slug: fairvalid-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-jobs-api-openapi.yml
- filename: fairvalid-com-simulator-api-openapi.yml
  format: yaml
  label: FairValid Simulator API
  slug: fairvalid-com-simulator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairvalid-com/openapi/fairvalid-com-simulator-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FairValid Authentication
name_suffix: Authentication
oauth_flows: []
overview: FairValid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FairValid
provider_slug: fairvalid-com
scheme_count: 1
schemes:
- bearerFormat: fv_live_ or fv_test_ server-side key
  description: Use one scoped key in Authorization. Secrets appear once at creation; never put them in a browser or mobile app.
  name: FairValidKey
  scheme: bearer
  sources:
  - openapi/fairvalid-com-openapi.json
  type: http
slug: fairvalid-com-authentication
source_filename: fairvalid-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/fairvalid-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: FairValidKey\n  type: http\n  scheme: bearer\n  bearerFormat: fv_live_ or fv_test_ server-side key\n  description: Use one scoped key in Authorization. Secrets appear once at creation; never put\n    them in a browser or mobile app.\n  sources:\n  - openapi/fairvalid-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fairvalid-com/authentication/fairvalid-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Verification
- Contact Search
- Sales
- Marketing
---
