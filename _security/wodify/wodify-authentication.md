---
api_key_in: []
api_specs:
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Clients API
  slug: wodify-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Leads API
  slug: wodify-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Memberships API
  slug: wodify-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Classes and Programs API
  slug: wodify-classes-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Workouts and Performance API
  slug: wodify-workouts-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Services and Appointments API
  slug: wodify-services-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Financials API
  slug: wodify-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
- filename: wodify-openapi.yml
  format: yaml
  label: Wodify Communications API
  slug: wodify-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wodify/refs/heads/main/openapi/wodify-openapi.yml
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
