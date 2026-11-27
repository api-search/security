---
anonymous_access: false
api_key_in: []
api_specs:
- filename: temporevenue-com-credits-api-openapi.yml
  format: yaml
  label: TempoRevenue Credits API
  slug: temporevenue-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temporevenue-com/openapi/temporevenue-com-credits-api-openapi.yml
- filename: temporevenue-com-proposals-api-openapi.yml
  format: yaml
  label: TempoRevenue Proposals API
  slug: temporevenue-com-proposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temporevenue-com/openapi/temporevenue-com-proposals-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: TempoRevenue Authentication
name_suffix: Authentication
oauth_flows: []
overview: TempoRevenue secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TempoRevenue
provider_slug: temporevenue-com
scheme_count: 1
schemes:
- bearerFormat: tr_live_...
  description: 'API key created in Integrations in the TempoRevenue app. Send it as Authorization: Bearer tr_live_... Keys are shown once and can be revoked anytime. Up to 5 active keys per account.'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/temporevenue-com-openapi.json
  type: http
slug: temporevenue-com-authentication
source_filename: temporevenue-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/temporevenue-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: tr_live_...\n  description: 'API key created in Integrations in the TempoRevenue app. Send it as Authorization:\n    Bearer tr_live_... Keys are shown once and can be revoked anytime. Up to 5 active keys per\n    account.'\n  sources:\n  - openapi/temporevenue-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/temporevenue-com/authentication/temporevenue-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Contract
- Automation
- Freelance
- SmallBusiness
---
