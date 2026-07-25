---
api_key_in:
- query
api_specs:
- filename: food-and-drug-administration-animal-veterinary-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Animal & Veterinary API
  slug: food-and-drug-administration-animal-veterinary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-animal-veterinary-api-openapi.yml
- filename: food-and-drug-administration-device-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Device API
  slug: food-and-drug-administration-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-device-api-openapi.yml
- filename: food-and-drug-administration-drug-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Drug API
  slug: food-and-drug-administration-drug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-drug-api-openapi.yml
- filename: food-and-drug-administration-food-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Food API
  slug: food-and-drug-administration-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-food-api-openapi.yml
- filename: food-and-drug-administration-other-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Other API
  slug: food-and-drug-administration-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-other-api-openapi.yml
- filename: food-and-drug-administration-tobacco-api-openapi.yml
  format: yaml
  label: Food and Drug Administration Tobacco API
  slug: food-and-drug-administration-tobacco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/openapi/food-and-drug-administration-tobacco-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Food And Drug Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Food and Drug Administration secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Food and Drug Administration
provider_slug: food-and-drug-administration
scheme_count: 1
schemes:
- description: 'Free openFDA API key (obtain at https://open.fda.gov/apis/authentication/). Without a key: 240 req/min and 1,000 req/day per IP. With a key: 240 req/min and 120,000 req/day per key.'
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/openfda-openapi.yml
  type: apiKey
slug: food-and-drug-administration-authentication
source_filename: food-and-drug-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openfda-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 'Free openFDA API key (obtain at https://open.fda.gov/apis/authentication/).\n    Without a key: 240 req/min and 1,000 req/day per IP. With a key: 240 req/min and 120,000\n    req/day per key.'\n  sources:\n  - openapi/openfda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-and-drug-administration/refs/heads/main/authentication/food-and-drug-administration-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Drugs
- Devices
- Federal Government
- Food Safety
- Public Data
- Recalls
- Adverse Events
---
