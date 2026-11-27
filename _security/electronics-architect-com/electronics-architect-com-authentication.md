---
anonymous_access: false
api_key_in: []
api_specs:
- filename: electronics-architect-com-account-api-openapi.yml
  format: yaml
  label: Electronics Architect Account API
  slug: electronics-architect-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-account-api-openapi.yml
- filename: electronics-architect-com-ai-api-openapi.yml
  format: yaml
  label: Electronics Architect AI API
  slug: electronics-architect-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-ai-api-openapi.yml
- filename: electronics-architect-com-compare-api-openapi.yml
  format: yaml
  label: Electronics Architect Compare API
  slug: electronics-architect-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-compare-api-openapi.yml
- filename: electronics-architect-com-designs-api-openapi.yml
  format: yaml
  label: Electronics Architect Designs API
  slug: electronics-architect-com-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-designs-api-openapi.yml
- filename: electronics-architect-com-exports-api-openapi.yml
  format: yaml
  label: Electronics Architect Exports API
  slug: electronics-architect-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-exports-api-openapi.yml
- filename: electronics-architect-com-jobs-api-openapi.yml
  format: yaml
  label: Electronics Architect Jobs API
  slug: electronics-architect-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-jobs-api-openapi.yml
- filename: electronics-architect-com-library-api-openapi.yml
  format: yaml
  label: Electronics Architect Library API
  slug: electronics-architect-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-library-api-openapi.yml
- filename: electronics-architect-com-solve-api-openapi.yml
  format: yaml
  label: Electronics Architect Solve API
  slug: electronics-architect-com-solve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-solve-api-openapi.yml
- filename: electronics-architect-com-templates-api-openapi.yml
  format: yaml
  label: Electronics Architect Templates API
  slug: electronics-architect-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electronics-architect-com/openapi/electronics-architect-com-templates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Electronics Architect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electronics Architect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Electronics Architect
provider_slug: electronics-architect-com
scheme_count: 1
schemes:
- bearerFormat: ea_live_…
  description: An API key from Account → Developer in the editor (Pro and Team plans), or the key an MCP client's OAuth sign-in mints (any plan; a Free account's key carries the Free limits).
  name: apiKey
  scheme: bearer
  sources:
  - openapi/electronics-architect-com-openapi.json
  type: http
slug: electronics-architect-com-authentication
source_filename: electronics-architect-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/electronics-architect-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ea_live_…\n  description: An API key from Account → Developer in the editor (Pro and Team plans), or the\n    key an MCP client's OAuth sign-in mints (any plan; a Free account's key carries the Free\n    limits).\n  sources:\n  - openapi/electronics-architect-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/electronics-architect-com/authentication/electronics-architect-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Power Design
- Electrical Engineering
- Software-as-a-Service
- Simulation
---
