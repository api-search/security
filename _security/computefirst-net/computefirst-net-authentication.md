---
anonymous_access: false
api_key_in: []
api_specs:
- filename: computefirst-net-account-api-openapi.yml
  format: yaml
  label: ComputeFirst Account API
  slug: computefirst-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-account-api-openapi.yml
- filename: computefirst-net-discovery-api-openapi.yml
  format: yaml
  label: ComputeFirst Discovery API
  slug: computefirst-net-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-discovery-api-openapi.yml
- filename: computefirst-net-execution-api-openapi.yml
  format: yaml
  label: ComputeFirst Execution API
  slug: computefirst-net-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-execution-api-openapi.yml
- filename: computefirst-net-feedback-api-openapi.yml
  format: yaml
  label: ComputeFirst Feedback API
  slug: computefirst-net-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-feedback-api-openapi.yml
- filename: computefirst-net-mcp-api-openapi.yml
  format: yaml
  label: ComputeFirst MCP API
  slug: computefirst-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-mcp-api-openapi.yml
- filename: computefirst-net-newsletter-api-openapi.yml
  format: yaml
  label: ComputeFirst Newsletter API
  slug: computefirst-net-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-newsletter-api-openapi.yml
- filename: computefirst-net-savings-api-openapi.yml
  format: yaml
  label: ComputeFirst Savings API
  slug: computefirst-net-savings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-savings-api-openapi.yml
- filename: computefirst-net-service-api-openapi.yml
  format: yaml
  label: ComputeFirst Service API
  slug: computefirst-net-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/computefirst-net/openapi/computefirst-net-service-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ComputeFirst Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComputeFirst secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ComputeFirst
provider_slug: computefirst-net
scheme_count: 1
schemes:
- description: Optional key from email sign-in or a passkey profile. Not needed for search, contracts or execution.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/computefirst-net-openapi.yml
  type: http
slug: computefirst-net-authentication
source_filename: computefirst-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/computefirst-net-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional key from email sign-in or a passkey profile. Not needed for search,\n    contracts or execution.\n  sources:\n  - openapi/computefirst-net-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/computefirst-net/authentication/computefirst-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Agents
- MCP
- Developer Tools
- Data Transformation
- CSV
- JSON
- Deterministic Tools
---
