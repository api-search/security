---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sipi-agents-api-openapi.yml
  format: yaml
  label: GitDealFlow Agents API
  slug: sipi-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-agents-api-openapi.yml
- filename: sipi-approvals-api-openapi.yml
  format: yaml
  label: GitDealFlow Approvals API
  slug: sipi-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-approvals-api-openapi.yml
- filename: sipi-budget-api-openapi.yml
  format: yaml
  label: GitDealFlow Budget API
  slug: sipi-budget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-budget-api-openapi.yml
- filename: sipi-evaluate-api-openapi.yml
  format: yaml
  label: GitDealFlow Evaluate API
  slug: sipi-evaluate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-evaluate-api-openapi.yml
- filename: sipi-rules-api-openapi.yml
  format: yaml
  label: GitDealFlow Rules API
  slug: sipi-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-rules-api-openapi.yml
- filename: sipi-system-api-openapi.yml
  format: yaml
  label: GitDealFlow System API
  slug: sipi-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-system-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sipi Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitDealFlow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GitDealFlow
provider_slug: sipi
scheme_count: 1
schemes:
- description: A checkout-issued or operator-created API key. ADMIN_TOKEN is accepted only for operator control-plane access.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sipi-openapi.json
  type: http
slug: sipi-authentication
source_filename: sipi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/sipi-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: A checkout-issued or operator-created API key. ADMIN_TOKEN is accepted only for\n    operator control-plane access.\n  sources:\n  - openapi/sipi-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/sipi/authentication/sipi-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Finance
- Security
- Automation
- Software-as-a-Service
---
