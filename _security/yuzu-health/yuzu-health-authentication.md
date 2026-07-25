---
api_key_in: []
api_specs:
- filename: yuzu-health-accumulator-experimental-api-openapi.yml
  format: yaml
  label: Yuzu Health Accumulator (Experimental) API
  slug: yuzu-health-accumulator-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-accumulator-experimental-api-openapi.yml
- filename: yuzu-health-benefits-api-openapi.yml
  format: yaml
  label: Yuzu Health Benefits API
  slug: yuzu-health-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-benefits-api-openapi.yml
- filename: yuzu-health-coverage-api-openapi.yml
  format: yaml
  label: Yuzu Health Coverage API
  slug: yuzu-health-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-coverage-api-openapi.yml
- filename: yuzu-health-enrollment-api-openapi.yml
  format: yaml
  label: Yuzu Health Enrollment API
  slug: yuzu-health-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-enrollment-api-openapi.yml
- filename: yuzu-health-eob-experimental-api-openapi.yml
  format: yaml
  label: Yuzu Health EOB (Experimental) API
  slug: yuzu-health-eob-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-eob-experimental-api-openapi.yml
- filename: yuzu-health-group-policy-api-openapi.yml
  format: yaml
  label: Yuzu Health Group Policy API
  slug: yuzu-health-group-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-group-policy-api-openapi.yml
- filename: yuzu-health-member-api-openapi.yml
  format: yaml
  label: Yuzu Health Member API
  slug: yuzu-health-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-member-api-openapi.yml
- filename: yuzu-health-publicapiv1-api-openapi.yml
  format: yaml
  label: Yuzu Health PublicApiV1 API
  slug: yuzu-health-publicapiv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-publicapiv1-api-openapi.yml
- filename: yuzu-health-publicapiv2-api-openapi.yml
  format: yaml
  label: Yuzu Health PublicApiV2 API
  slug: yuzu-health-publicapiv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-publicapiv2-api-openapi.yml
- filename: yuzu-health-sponsor-api-openapi.yml
  format: yaml
  label: Yuzu Health Sponsor API
  slug: yuzu-health-sponsor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-sponsor-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Yuzu Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yuzu Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yuzu Health
provider_slug: yuzu-health
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: public-api-auth
  scheme: bearer
  sources:
  - openapi/yuzu-health-openapi-original.json
  type: http
slug: yuzu-health-authentication
source_filename: yuzu-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/yuzu-health-openapi-original.json\ndocs: https://yuzu.health/docs/guides/api\nnotes: API keys are minted in the vendor portal (Settings > Developer), each key maps to an owning\n  org/employee, and are passed as a bearer token (JWT) in the Authorization header.\nsummary:\n  types:\n  - http\nschemes:\n- name: public-api-auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/yuzu-health-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/authentication/yuzu-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Healthcare
- Insurance
- Health Plans
- Benefits Administration
- Claims
- Enrollment
- Payers
- Self-Funded
---
