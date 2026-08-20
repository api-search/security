---
api_key_in:
- header
api_specs:
- filename: nutrical-solution-ltd-entity-api-openapi.yml
  format: yaml
  label: Nutrical Solution Ltd Entity API
  slug: nutrical-solution-ltd-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-entity-api-openapi.yml
- filename: nutrical-solution-ltd-ingredients-api-openapi.yml
  format: yaml
  label: Nutrical Solution Ltd Ingredients API
  slug: nutrical-solution-ltd-ingredients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-ingredients-api-openapi.yml
- filename: nutrical-solution-ltd-meal-plans-api-openapi.yml
  format: yaml
  label: Nutrical Solution Ltd Meal Plans API
  slug: nutrical-solution-ltd-meal-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-meal-plans-api-openapi.yml
- filename: nutrical-solution-ltd-metadata-api-openapi.yml
  format: yaml
  label: Nutrical Solution Ltd Metadata API
  slug: nutrical-solution-ltd-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-metadata-api-openapi.yml
- filename: nutrical-solution-ltd-recipe-categories-api-openapi.yml
  format: yaml
  label: Nutrical Solution Ltd Recipe Categories API
  slug: nutrical-solution-ltd-recipe-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-recipe-categories-api-openapi.yml
- filename: nutrical-solution-ltd-recipes-api-openapi.yml
  format: yaml
  label: Nutrical Solution Ltd Recipes API
  slug: nutrical-solution-ltd-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-recipes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nutrical Solution Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nutrical Solution Ltd secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nutrical Solution Ltd
provider_slug: nutrical-solution-ltd
scheme_count: 2
schemes:
- description: Entity client access token issued by the Create Entity operation.
  in: header
  name: AccessToken
  parameter: Access-Token
  sources:
  - openapi/nutrical-solution-ltd-openapi.yml
  type: apiKey
- description: Organization-level API key (documented header name "API Key"), used to provision entities via the Create Entity operation.
  in: header
  name: ApiKey
  parameter: API Key
  sources:
  - openapi/nutrical-solution-ltd-openapi.yml
  type: apiKey
slug: nutrical-solution-ltd-authentication
source_filename: nutrical-solution-ltd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nutrical-solution-ltd-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  description: Entity client access token issued by the Create Entity operation.\n  sources:\n  - openapi/nutrical-solution-ltd-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: API Key\n  description: Organization-level API key (documented header name \"API Key\"), used to provision\n    entities via the Create Entity operation.\n  sources:\n  - openapi/nutrical-solution-ltd-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/authentication/nutrical-solution-ltd-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Food
- Nutrition
- Health
- Recipes
- Meal Plans
- Food Labeling
- Compliance
- Restaurant
- GCC
---
