---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meal-planner-online.openapi.json
  format: json
  label: Meal Planner Read-only API
  slug: meal-planner-read-only-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meal-planner-online/openapi/meal-planner-online.openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Meal Planner Online Authentication
name_suffix: Authentication
oauth_flows: []
overview: meal-planner-online secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: meal-planner-online
provider_slug: meal-planner-online
scheme_count: 1
schemes:
- bearerFormat: mp_ro_ID.SECRET
  description: Read-only token. Send only in Authorization; credentials in URLs are rejected.
  name: MealPlannerToken
  scheme: bearer
  sources:
  - openapi/meal-planner-online.openapi.json
  type: http
slug: meal-planner-online-authentication
source_filename: meal-planner-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/meal-planner-online.openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: MealPlannerToken\n  type: http\n  scheme: bearer\n  bearerFormat: mp_ro_ID.SECRET\n  description: Read-only token. Send only in Authorization; credentials in URLs are rejected.\n  sources:\n  - openapi/meal-planner-online.openapi.json\n"
source_yaml_url: https://artifacts.apis.io/meal-planner-online/authentication/meal-planner-online-authentication.yml
summary_line: http · 1 scheme
tags:
- Meal Planning
- Family
- Canada
- API
- Subscription
- Cooking
---
