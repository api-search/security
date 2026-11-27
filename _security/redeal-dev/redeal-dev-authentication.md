---
anonymous_access: false
api_key_in: []
api_specs:
- filename: redeal-dev-certificates-api-openapi.yml
  format: yaml
  label: Redeal Certificates API
  slug: redeal-dev-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-certificates-api-openapi.yml
- filename: redeal-dev-deals-api-openapi.yml
  format: yaml
  label: Redeal Deals API
  slug: redeal-dev-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-deals-api-openapi.yml
- filename: redeal-dev-onboarding-api-openapi.yml
  format: yaml
  label: Redeal Onboarding API
  slug: redeal-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-onboarding-api-openapi.yml
- filename: redeal-dev-transparency-api-openapi.yml
  format: yaml
  label: Redeal Transparency API
  slug: redeal-dev-transparency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-transparency-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Redeal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Redeal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Redeal
provider_slug: redeal-dev
scheme_count: 1
schemes:
- description: API key (fp_...) for initiator actions; invite token for party actions
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/redeal-dev-openapi.json
  type: http
slug: redeal-dev-authentication
source_filename: redeal-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: derived\nsource: openapi/redeal-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key (fp_...) for initiator actions; invite token for party actions\n  sources:\n  - openapi/redeal-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/redeal-dev/authentication/redeal-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Fairness Computation
- API
- Sealed‑Bid Auction
- Shapley Value
- Verification
---
