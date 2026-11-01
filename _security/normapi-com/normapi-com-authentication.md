---
anonymous_access: false
api_key_in: []
api_specs:
- filename: normapi-com-openapi.yml
  format: yaml
  label: NormAPI REST API
  slug: normapi-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normapi-com/openapi/normapi-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Normapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: NormAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NormAPI
provider_slug: normapi-com
scheme_count: 1
schemes:
- description: 'Your API key from the dashboard, as `Authorization: Bearer nk_live_…`.

    Validation also works without one, under anonymous rate limits.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/normapi-com-customers-api-openapi.yml
  - openapi/normapi-com-generation-api-openapi.yml
  - openapi/normapi-com-parsing-api-openapi.yml
  - openapi/normapi-com-validation-api-openapi.yml
  type: http
slug: normapi-com-authentication
source_filename: normapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: derived\nsource: openapi/normapi-com-customers-api-openapi.yml, openapi/normapi-com-generation-api-openapi.yml,\n  openapi/normapi-com-parsing-api-openapi.yml, openapi/normapi-com-validation-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Your API key from the dashboard, as `Authorization: Bearer nk_live_…`.\n    Validation also works without one, under anonymous rate limits.\n  sources:\n  - openapi/normapi-com-customers-api-openapi.yml\n  - openapi/normapi-com-generation-api-openapi.yml\n  - openapi/normapi-com-parsing-api-openapi.yml\n  - openapi/normapi-com-validation-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/normapi-com/authentication/normapi-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- e-invoicing
- XRechnung
- ZUGFeRD
- Germany
---
