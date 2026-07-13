---
api_key_in:
- query
api_specs:
- filename: applitools-openapi.yml
  format: yaml
  label: Applitools Eyes Server REST API
  slug: eyes-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applitools/refs/heads/main/openapi/applitools-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Applitools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Applitools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Applitools
provider_slug: applitools
scheme_count: 1
schemes:
- description: Applitools API key passed as a query parameter.
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/applitools-openapi.yml
  type: apiKey
slug: applitools-authentication
source_filename: applitools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/applitools-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Applitools API key passed as a query parameter.\n  sources:\n  - openapi/applitools-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applitools/refs/heads/main/authentication/applitools-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Testing
- Visual AI
- Visual Testing
- Autonomous Testing
- REST
- SDK
- Cross-Browser
- Execution Cloud
---
