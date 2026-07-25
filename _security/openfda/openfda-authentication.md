---
api_key_in:
- query
api_specs:
- filename: openfda-animal-veterinary-api-openapi.yml
  format: yaml
  label: openFDA Animal & Veterinary API
  slug: openfda-animal-veterinary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-animal-veterinary-api-openapi.yml
- filename: openfda-device-api-openapi.yml
  format: yaml
  label: openFDA Device API
  slug: openfda-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-device-api-openapi.yml
- filename: openfda-drug-api-openapi.yml
  format: yaml
  label: openFDA Drug API
  slug: openfda-drug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-drug-api-openapi.yml
- filename: openfda-food-api-openapi.yml
  format: yaml
  label: openFDA Food API
  slug: openfda-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-food-api-openapi.yml
- filename: openfda-other-api-openapi.yml
  format: yaml
  label: openFDA Other API
  slug: openfda-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-other-api-openapi.yml
- filename: openfda-tobacco-api-openapi.yml
  format: yaml
  label: openFDA Tobacco API
  slug: openfda-tobacco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-tobacco-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openfda Authentication
name_suffix: Authentication
oauth_flows: []
overview: openFDA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: openFDA
provider_slug: openfda
scheme_count: 1
schemes:
- description: 'Free openFDA API key (obtain at https://open.fda.gov/apis/authentication/). Without a key: 240 req/min and 1,000 req/day per IP. With a key: 240 req/min and 120,000 req/day per key.'
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/openfda-openapi.yml
  type: apiKey
slug: openfda-authentication
source_filename: openfda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openfda-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 'Free openFDA API key (obtain at https://open.fda.gov/apis/authentication/).\n    Without a key: 240 req/min and 1,000 req/day per IP. With a key: 240 req/min and 120,000\n    req/day per key.'\n  sources:\n  - openapi/openfda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/authentication/openfda-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Healthcare
- Drug
- Device
- Food
- Animal & Veterinary
- Tobacco
- Public Data
- Open Data
- Adverse Events
- Recalls
- Regulatory
---
