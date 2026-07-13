---
api_key_in:
- header
api_specs:
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq Datasource API
  slug: altruistiq-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq PACT API
  slug: altruistiq-pact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Altruistiq Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Altruistiq secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Altruistiq
provider_slug: altruistiq
scheme_count: 2
schemes:
- description: 'Enter the token with the `Bearer: ` prefix, e.g. `Bearer: apiKey`.'
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/altruistiq-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  sources:
  - openapi/altruistiq-openapi.yml
  type: oauth2
slug: altruistiq-authentication
source_filename: altruistiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/altruistiq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Enter the token with the `Bearer: ` prefix, e.g. `Bearer: apiKey`.'\n  sources:\n  - openapi/altruistiq-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/altruistiq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/authentication/altruistiq-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Sustainability
- Climate
- Carbon Accounting
- Emissions
- Greenhouse Gas
- Scope 3
- Product Carbon Footprint
- Corporate Carbon Footprint
- Supply Chain
- FMCG
- Food and Beverage
- ESG
- CSRD
- SBTi
- PACT
- Sustainability Intelligence
---
