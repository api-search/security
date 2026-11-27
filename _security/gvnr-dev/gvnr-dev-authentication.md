---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gvnr-dev-account-api-openapi.yml
  format: yaml
  label: Gvnr Account API
  slug: gvnr-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-account-api-openapi.yml
- filename: gvnr-dev-approval-api-openapi.yml
  format: yaml
  label: Gvnr Approval API
  slug: gvnr-dev-approval-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-approval-api-openapi.yml
- filename: gvnr-dev-approve-api-openapi.yml
  format: yaml
  label: Gvnr Approve API
  slug: gvnr-dev-approve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-approve-api-openapi.yml
- filename: gvnr-dev-budget-api-openapi.yml
  format: yaml
  label: Gvnr Budget API
  slug: gvnr-dev-budget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-budget-api-openapi.yml
- filename: gvnr-dev-idempotency-api-openapi.yml
  format: yaml
  label: Gvnr Idempotency API
  slug: gvnr-dev-idempotency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-idempotency-api-openapi.yml
- filename: gvnr-dev-mcp-api-openapi.yml
  format: yaml
  label: Gvnr MCP API
  slug: gvnr-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-mcp-api-openapi.yml
- filename: gvnr-dev-packs-api-openapi.yml
  format: yaml
  label: Gvnr Packs API
  slug: gvnr-dev-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-packs-api-openapi.yml
- filename: gvnr-dev-rate-api-openapi.yml
  format: yaml
  label: Gvnr Rate API
  slug: gvnr-dev-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gvnr-dev/openapi/gvnr-dev-rate-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gvnr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gvnr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gvnr
provider_slug: gvnr-dev
scheme_count: 1
schemes:
- description: API key from POST /v1/account
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gvnr-dev-openapi.json
  type: http
slug: gvnr-dev-authentication
source_filename: gvnr-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gvnr-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from POST /v1/account\n  sources:\n  - openapi/gvnr-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gvnr-dev/authentication/gvnr-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Budgets
- SpendControl
- MCP
- Finance
---
