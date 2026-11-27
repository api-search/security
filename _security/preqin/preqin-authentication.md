---
anonymous_access: false
api_key_in: []
api_specs:
- filename: preqin-active-user-subscription-info-api-openapi.yml
  format: yaml
  label: Preqin Active User Subscription Info API
  slug: preqin-active-user-subscription-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-active-user-subscription-info-api-openapi.yml
- filename: preqin-connect-api-openapi.yml
  format: yaml
  label: Preqin Connect API
  slug: preqin-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-connect-api-openapi.yml
- filename: preqin-deal-api-openapi.yml
  format: yaml
  label: Preqin Deal API
  slug: preqin-deal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-deal-api-openapi.yml
- filename: preqin-fund-api-openapi.yml
  format: yaml
  label: Preqin Fund API
  slug: preqin-fund-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-fund-api-openapi.yml
- filename: preqin-fund-manager-api-openapi.yml
  format: yaml
  label: Preqin Fund Manager API
  slug: preqin-fund-manager-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-fund-manager-api-openapi.yml
- filename: preqin-fund-performance-api-openapi.yml
  format: yaml
  label: Preqin Fund Performance API
  slug: preqin-fund-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-fund-performance-api-openapi.yml
- filename: preqin-investment-consultant-api-openapi.yml
  format: yaml
  label: Preqin Investment Consultant API
  slug: preqin-investment-consultant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-investment-consultant-api-openapi.yml
- filename: preqin-investor-api-openapi.yml
  format: yaml
  label: Preqin Investor API
  slug: preqin-investor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-investor-api-openapi.yml
- filename: preqin-investor-commitment-add-on-api-openapi.yml
  format: yaml
  label: Preqin Investor Commitment (Add-on) API
  slug: preqin-investor-commitment-add-on-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-investor-commitment-add-on-api-openapi.yml
- filename: preqin-news-api-openapi.yml
  format: yaml
  label: Preqin News API
  slug: preqin-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-news-api-openapi.yml
- filename: preqin-service-provider-api-openapi.yml
  format: yaml
  label: Preqin Service Provider API
  slug: preqin-service-provider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-service-provider-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Preqin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Preqin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Preqin
provider_slug: preqin
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: See the Authentication section of the documentation to obtain a token, and then paste it below
  name: bearer
  scheme: Bearer
  sources:
  - openapi/preqin-openapi.json
  type: http
slug: preqin-authentication
source_filename: preqin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/preqin-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: See the Authentication section of the documentation to obtain a token, and then\n    paste it below\n  sources:\n  - openapi/preqin-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/preqin/authentication/preqin-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Alternative Assets
- Data
- Analytics
- Private Markets
- Research
---
