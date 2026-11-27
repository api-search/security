---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: symphony-fr-baskets-api-openapi.yml
  format: yaml
  label: Symphony Baskets API
  slug: symphony-fr-baskets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-baskets-api-openapi.yml
- filename: symphony-fr-ingredients-api-openapi.yml
  format: yaml
  label: Symphony Ingredients API
  slug: symphony-fr-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-ingredients-api-openapi.yml
- filename: symphony-fr-recipes-api-openapi.yml
  format: yaml
  label: Symphony Recipes API
  slug: symphony-fr-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-recipes-api-openapi.yml
- filename: symphony-fr-users-api-openapi.yml
  format: yaml
  label: Symphony Users API
  slug: symphony-fr-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symphony-fr/openapi/symphony-fr-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Symphony Authentication
name_suffix: Authentication
oauth_flows: []
overview: Symphony secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Symphony
provider_slug: symphony-fr
scheme_count: 1
schemes:
- description: 'API key for authentication. Obtain from: https://symphony.fr/en/my-account/account/api-keys

    Include as ''api_key'' query parameter in all requests'
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/symphony-fr-openapi.yml
  type: apiKey
slug: symphony-fr-authentication
source_filename: symphony-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/symphony-fr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: |-\n    API key for authentication. Obtain from: https://symphony.fr/en/my-account/account/api-keys\n    Include as 'api_key' query parameter in all requests\n  sources:\n  - openapi/symphony-fr-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/symphony-fr/authentication/symphony-fr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Meal Delivery
- Nutrition
- Personalized Meals
- French Startup
- Health Tech
---
