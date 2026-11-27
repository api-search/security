---
anonymous_access: false
api_key_in: []
api_specs:
- filename: noozra-building-permits-api-openapi.yml
  format: yaml
  label: Noozra Building permits API
  slug: noozra-building-permits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-building-permits-api-openapi.yml
- filename: noozra-communities-api-openapi.yml
  format: yaml
  label: Noozra Communities API
  slug: noozra-communities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-communities-api-openapi.yml
- filename: noozra-datasets-api-openapi.yml
  format: yaml
  label: Noozra Datasets API
  slug: noozra-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-datasets-api-openapi.yml
- filename: noozra-federal-register-api-openapi.yml
  format: yaml
  label: Noozra Federal Register API
  slug: noozra-federal-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-federal-register-api-openapi.yml
- filename: noozra-government-contracts-api-openapi.yml
  format: yaml
  label: Noozra Government contracts API
  slug: noozra-government-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-government-contracts-api-openapi.yml
- filename: noozra-jobs-api-openapi.yml
  format: yaml
  label: Noozra Jobs API
  slug: noozra-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-jobs-api-openapi.yml
- filename: noozra-new-businesses-api-openapi.yml
  format: yaml
  label: Noozra New businesses API
  slug: noozra-new-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-new-businesses-api-openapi.yml
- filename: noozra-news-api-openapi.yml
  format: yaml
  label: Noozra News API
  slug: noozra-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-news-api-openapi.yml
- filename: noozra-product-recalls-api-openapi.yml
  format: yaml
  label: Noozra Product recalls API
  slug: noozra-product-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noozra/openapi/noozra-product-recalls-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Noozra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noozra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Noozra
provider_slug: noozra
scheme_count: 1
schemes:
- description: 'API key (nk_…), from a free account: https://noozra.com/register?next=%2Faccount%2Fapi. A new free key needs a card saved to the account; saving it charges nothing. Free (100/day, personal and non-commercial use) or API Pro (25,000/day, commercial use of the API and the archive). Required on every request except /api/categories and /api/datasets.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/noozra-openapi.json
  type: http
slug: noozra-authentication
source_filename: noozra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/noozra-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key (nk_…), from a free account: https://noozra.com/register?next=%2Faccount%2Fapi.\n    A new free key needs a card saved to the account; saving it charges nothing. Free (100/day,\n    personal and non-commercial use) or API Pro (25,000/day, commercial use of the API and the\n    archive). Required on every request except /api/categories and /api/datasets.'\n  sources:\n  - openapi/noozra-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/noozra/authentication/noozra-authentication.yml
summary_line: http · 1 scheme
tags:
- News
- Free
- Community
- Artificial Intelligence
---
