---
api_key_in: []
api_specs:
- filename: databook-openapi-original.json
  format: json
  label: DatabookAI REST API
  slug: databookai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Databook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Databook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Databook
provider_slug: databook
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/databook-openapi-original.json
  type: http
slug: databook-authentication
source_filename: databook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/databook-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/databook-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/authentication/databook-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Vertical Software
- Sales Intelligence
- Account Intelligence
- Sales Enablement
- Enterprise Sales
- Artificial Intelligence
- Revenue Operations
- REST API
- OpenAPI
- Batch Processing
- Agents
- Reasoning
- Company Data
---
