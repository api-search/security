---
api_key_in:
- header
api_specs:
- filename: centers-for-disease-control-and-prevention-openapi.yml
  format: yaml
  label: CDC Socrata Open Data API (data.cdc.gov)
  slug: cdc-socrata-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Centers For Disease Control And Prevention Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centers for Disease Control and Prevention secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Centers for Disease Control and Prevention
provider_slug: centers-for-disease-control-and-prevention
scheme_count: 1
schemes:
- description: 'Socrata application token. Anonymous use is allowed at throttled rates;

    an app token raises rate limits. May also be supplied as the

    $$app_token query parameter.'
  in: header
  name: appToken
  parameter: X-App-Token
  sources:
  - openapi/centers-for-disease-control-and-prevention-openapi.yml
  type: apiKey
slug: centers-for-disease-control-and-prevention-authentication
source_filename: centers-for-disease-control-and-prevention-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/centers-for-disease-control-and-prevention-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: |-\n    Socrata application token. Anonymous use is allowed at throttled rates;\n    an app token raises rate limits. May also be supplied as the\n    $$app_token query parameter.\n  sources:\n  - openapi/centers-for-disease-control-and-prevention-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/authentication/centers-for-disease-control-and-prevention-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CDC
- Environmental Health
- Epidemiology
- Federal Government
- Healthcare
- Open Data
- Public Health
- Socrata
- Surveillance
- WONDER
---
