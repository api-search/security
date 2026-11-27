---
anonymous_access: false
api_key_in: []
api_specs:
- filename: geniusdecision-app-agents-api-openapi.yml
  format: yaml
  label: Genius Decision App Agents API
  slug: geniusdecision-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-agents-api-openapi.yml
- filename: geniusdecision-app-cases-api-openapi.yml
  format: yaml
  label: Genius Decision App Cases API
  slug: geniusdecision-app-cases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-cases-api-openapi.yml
- filename: geniusdecision-app-choice-api-openapi.yml
  format: yaml
  label: Genius Decision App Choice API
  slug: geniusdecision-app-choice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-choice-api-openapi.yml
- filename: geniusdecision-app-config-api-openapi.yml
  format: yaml
  label: Genius Decision App Config API
  slug: geniusdecision-app-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-config-api-openapi.yml
- filename: geniusdecision-app-examples-api-openapi.yml
  format: yaml
  label: Genius Decision App Examples API
  slug: geniusdecision-app-examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-examples-api-openapi.yml
- filename: geniusdecision-app-health-api-openapi.yml
  format: yaml
  label: Genius Decision App Health API
  slug: geniusdecision-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-health-api-openapi.yml
- filename: geniusdecision-app-jobs-api-openapi.yml
  format: yaml
  label: Genius Decision App Jobs API
  slug: geniusdecision-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-jobs-api-openapi.yml
- filename: geniusdecision-app-me-api-openapi.yml
  format: yaml
  label: Genius Decision App Me API
  slug: geniusdecision-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-me-api-openapi.yml
- filename: geniusdecision-app-missions-api-openapi.yml
  format: yaml
  label: Genius Decision App Missions API
  slug: geniusdecision-app-missions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geniusdecision-app/openapi/geniusdecision-app-missions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Genius Decision App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genius Decision App secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Genius Decision App
provider_slug: geniusdecision-app
scheme_count: 1
schemes:
- description: HTTPS Authorization Bearer only. ga_ machine credentials carry enforced scopes and expiry for their own isolated space. gb_ human-account API keys retain full-account access. Neither is a JWT. No key in a query string.
  name: AccountBearer
  scheme: bearer
  sources:
  - openapi/geniusdecision-app-openapi.json
  type: http
slug: geniusdecision-app-authentication
source_filename: geniusdecision-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/geniusdecision-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: AccountBearer\n  type: http\n  scheme: bearer\n  description: HTTPS Authorization Bearer only. ga_ machine credentials carry enforced scopes\n    and expiry for their own isolated space. gb_ human-account API keys retain full-account\n    access. Neither is a JWT. No key in a query string.\n  sources:\n  - openapi/geniusdecision-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/geniusdecision-app/authentication/geniusdecision-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Decision-Making
- Sustainability
- Platform
---
