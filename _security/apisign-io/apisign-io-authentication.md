---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apisign-io-api-keys-api-openapi.yml
  format: yaml
  label: APISign API Keys API
  slug: apisign-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-api-keys-api-openapi.yml
- filename: apisign-io-contracts-api-openapi.yml
  format: yaml
  label: APISign Contracts API
  slug: apisign-io-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-contracts-api-openapi.yml
- filename: apisign-io-health-api-openapi.yml
  format: yaml
  label: APISign Health API
  slug: apisign-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-health-api-openapi.yml
- filename: apisign-io-organization-api-openapi.yml
  format: yaml
  label: APISign Organization API
  slug: apisign-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-organization-api-openapi.yml
- filename: apisign-io-templates-api-openapi.yml
  format: yaml
  label: APISign Templates API
  slug: apisign-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-templates-api-openapi.yml
- filename: apisign-io-webhooks-api-openapi.yml
  format: yaml
  label: APISign Webhooks API
  slug: apisign-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Apisign Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: APISign declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: APISign
provider_slug: apisign-io
scheme_count: 1
schemes:
- description: API key from the dashboard (Account → MCP & API Keys). Keys start with `ask_`.
  in: header
  name: x-api-key
  type: apiKey
slug: apisign-io-authentication
source_filename: apisign-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: https://apisign.io/api/openapi\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key from the dashboard (Account → MCP & API Keys). Keys start with `ask_`.\n"
source_yaml_url: https://artifacts.apis.io/apisign-io/authentication/apisign-io-authentication.yml
summary_line: 1 scheme
tags:
- E-Signature
- Artificial Intelligence
- MCP
- Contracts
- Developer Platform
---
