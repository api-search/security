---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: obolusfinanz-de-mcp-api-openapi.yml
  format: yaml
  label: Obolus MCP API
  slug: obolusfinanz-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-mcp-api-openapi.yml
- filename: obolusfinanz-de-resources-api-openapi.yml
  format: yaml
  label: Obolus Resources API
  slug: obolusfinanz-de-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-resources-api-openapi.yml
- filename: obolusfinanz-de-tools-api-openapi.yml
  format: yaml
  label: Obolus Tools API
  slug: obolusfinanz-de-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-tools-api-openapi.yml
- filename: obolusfinanz-de-open-api-api-openapi.yml
  format: yaml
  label: Obolus Open API
  slug: obolusfinanz-de-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-open-api-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Obolus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obolus secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Obolus
provider_slug: obolusfinanz-de
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-public-api-key
  sources:
  - openapi/obolusfinanz-de-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/obolusfinanz-de-openapi.yml
  type: http
slug: obolusfinanz-de-authentication
source_filename: obolusfinanz-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/obolusfinanz-de-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-public-api-key\n  sources:\n  - openapi/obolusfinanz-de-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/obolusfinanz-de-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/obolusfinanz-de/authentication/obolusfinanz-de-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Finance
- Relocation
- Tools
- Salary
---
