---
api_key_in: []
api_specs:
- filename: wodify-classes-api-openapi.yml
  format: yaml
  label: Wodify Classes API
  slug: wodify-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-classes-api-openapi.yml
- filename: wodify-clients-api-openapi.yml
  format: yaml
  label: Wodify Clients API
  slug: wodify-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-clients-api-openapi.yml
- filename: wodify-communications-api-openapi.yml
  format: yaml
  label: Wodify Communications API
  slug: wodify-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-communications-api-openapi.yml
- filename: wodify-financials-api-openapi.yml
  format: yaml
  label: Wodify Financials API
  slug: wodify-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-financials-api-openapi.yml
- filename: wodify-leads-api-openapi.yml
  format: yaml
  label: Wodify Leads API
  slug: wodify-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-leads-api-openapi.yml
- filename: wodify-memberships-api-openapi.yml
  format: yaml
  label: Wodify Memberships API
  slug: wodify-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-memberships-api-openapi.yml
- filename: wodify-programs-api-openapi.yml
  format: yaml
  label: Wodify Programs API
  slug: wodify-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-programs-api-openapi.yml
- filename: wodify-reference-api-openapi.yml
  format: yaml
  label: Wodify Reference API
  slug: wodify-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-reference-api-openapi.yml
- filename: wodify-services-api-openapi.yml
  format: yaml
  label: Wodify Services API
  slug: wodify-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-services-api-openapi.yml
- filename: wodify-workouts-api-openapi.yml
  format: yaml
  label: Wodify Workouts API
  slug: wodify-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-workouts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wodify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wodify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wodify
provider_slug: wodify
scheme_count: 1
schemes:
- description: A valid Wodify API key passed in the `x-api-key` request header. Customers using the Wodify Workflows feature already have a key (Wodify Core > Digital Presence > Web Integrations > API Keys, the key named "Wodify API"); partners request a key through the Wodify Developer Portal.
  in: header
  keyName: x-api-key
  name: apiKeyAuth
  sources:
  - openapi/wodify-openapi.yml
  - https://docs.wodify.com/docs/authentication
  type: apiKey
slug: wodify-authentication
source_filename: wodify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/wodify-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: x-api-key\n  description: >-\n    A valid Wodify API key passed in the `x-api-key` request header. Customers\n    using the Wodify Workflows feature already have a key (Wodify Core > Digital\n    Presence > Web Integrations > API Keys, the key named \"Wodify API\"); partners\n    request a key through the Wodify Developer Portal.\n  sources:\n  - openapi/wodify-openapi.yml\n  - https://docs.wodify.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/authentication/wodify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fitness
- Gym Management
- Membership Management
- Fitness Software
- CrossFit
- Class Scheduling
- Billing
- Wellness
- SaaS
---
