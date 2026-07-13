---
api_key_in: []
api_specs:
- filename: serif-health-openapi.yml
  format: yaml
  label: Serif Health Negotiated Rates API
  slug: negotiated-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serif-health/refs/heads/main/openapi/serif-health-openapi.yml
- filename: serif-health-openapi.yml
  format: yaml
  label: Serif Health Rate Distributions API
  slug: rate-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serif-health/refs/heads/main/openapi/serif-health-openapi.yml
- filename: serif-health-openapi.yml
  format: yaml
  label: Serif Health Find Care API
  slug: find-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serif-health/refs/heads/main/openapi/serif-health-openapi.yml
- filename: serif-health-openapi.yml
  format: yaml
  label: Serif Health Provider Directory API
  slug: provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serif-health/refs/heads/main/openapi/serif-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Serif Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Serif Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Serif Health
provider_slug: serif-health
scheme_count: 1
schemes:
- description: 'Serif Health API key passed as a Bearer token in the Authorization header (Authorization: Bearer <API_KEY>). API keys are issued by Serif Health; contact hello@serifhealth.com for access.'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/serif-health-openapi.yml
  type: http
slug: serif-health-authentication
source_filename: serif-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/serif-health-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Serif Health API key passed as a Bearer token in the Authorization header (Authorization:\n    Bearer <API_KEY>). API keys are issued by Serif Health; contact hello@serifhealth.com for\n    access.'\n  sources:\n  - openapi/serif-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serif-health/refs/heads/main/authentication/serif-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Price Transparency
- Negotiated Rates
- Payer
- Data
---
