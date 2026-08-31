---
api_key_in:
- header
api_specs:
- filename: uppsala-battledeaths-api-openapi.yml
  format: yaml
  label: Uppsala University BattleDeaths API
  slug: uppsala-battledeaths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-battledeaths-api-openapi.yml
- filename: uppsala-dyadic-api-openapi.yml
  format: yaml
  label: Uppsala University Dyadic API
  slug: uppsala-dyadic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-dyadic-api-openapi.yml
- filename: uppsala-gedevents-api-openapi.yml
  format: yaml
  label: Uppsala University GEDEvents API
  slug: uppsala-gedevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-gedevents-api-openapi.yml
- filename: uppsala-nonstate-api-openapi.yml
  format: yaml
  label: Uppsala University NonState API
  slug: uppsala-nonstate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-nonstate-api-openapi.yml
- filename: uppsala-onesided-api-openapi.yml
  format: yaml
  label: Uppsala University OneSided API
  slug: uppsala-onesided-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-onesided-api-openapi.yml
- filename: uppsala-organizedviolencecy-api-openapi.yml
  format: yaml
  label: Uppsala University OrganizedViolenceCY API
  slug: uppsala-organizedviolencecy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-organizedviolencecy-api-openapi.yml
- filename: uppsala-ucdpprioconflict-api-openapi.yml
  format: yaml
  label: Uppsala University UcdpPrioConflict API
  slug: uppsala-ucdpprioconflict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-ucdpprioconflict-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uppsala Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uppsala University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uppsala University
provider_slug: uppsala
scheme_count: 1
schemes:
- description: UCDP API token sent in x-ucdp-access-token header
  in: header
  name: ApiToken
  parameter: x-ucdp-access-token
  sources:
  - openapi/uppsala-ucdp.yaml
  type: apiKey
slug: uppsala-authentication
source_filename: uppsala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uppsala-ucdp.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: x-ucdp-access-token\n  description: UCDP API token sent in x-ucdp-access-token header\n  sources:\n  - openapi/uppsala-ucdp.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/authentication/uppsala-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- University
- Higher Education
- Education
- Sweden
- Public Research University
- Research Data
- Institutional Repository
- Identity Federation
- Research Computing
- Conflict Data
- Open Access
---
