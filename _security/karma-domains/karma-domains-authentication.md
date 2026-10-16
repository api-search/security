---
anonymous_access: false
api_key_in: []
api_specs:
- filename: karma-domains-domains-api-openapi.yml
  format: yaml
  label: Karma.Domains Domains API
  slug: karma-domains-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karma-domains/refs/heads/main/openapi/karma-domains-domains-api-openapi.yml
- filename: karma-domains-reports-api-openapi.yml
  format: yaml
  label: Karma.Domains Reports API
  slug: karma-domains-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karma-domains/refs/heads/main/openapi/karma-domains-reports-api-openapi.yml
- filename: karma-domains-user-api-openapi.yml
  format: yaml
  label: Karma.Domains User API
  slug: karma-domains-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karma-domains/refs/heads/main/openapi/karma-domains-user-api-openapi.yml
- filename: karma-domains-webhooks-api-openapi.yml
  format: yaml
  label: Karma.Domains Webhooks API
  slug: karma-domains-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karma-domains/refs/heads/main/openapi/karma-domains-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Karma Domains Authentication
name_suffix: Authentication
oauth_flows: []
overview: Karma.Domains secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Karma.Domains
provider_slug: karma-domains
scheme_count: 1
schemes:
- description: API key as Bearer token, or x402 PAYMENT-SIGNATURE for agent credits
  name: Bearer
  scheme: bearer
  sources:
  - openapi/karma-domains-openapi.json
  type: http
slug: karma-domains-authentication
source_filename: karma-domains-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: derived\nsource: openapi/karma-domains-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: API key as Bearer token, or x402 PAYMENT-SIGNATURE for agent credits\n  sources:\n  - openapi/karma-domains-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karma-domains/refs/heads/main/authentication/karma-domains-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SEO
- Domains
- Data
- API
---
