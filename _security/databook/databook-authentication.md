---
api_key_in: []
api_specs:
- filename: databook-batch-create-api-openapi.yml
  format: yaml
  label: Databook batch - create API
  slug: databook-batch-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-batch-create-api-openapi.yml
- filename: databook-batch-query-api-openapi.yml
  format: yaml
  label: Databook batch - query API
  slug: databook-batch-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-batch-query-api-openapi.yml
- filename: databook-chat-api-openapi.yml
  format: yaml
  label: Databook Chat API
  slug: databook-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-chat-api-openapi.yml
- filename: databook-reasoning-api-openapi.yml
  format: yaml
  label: Databook Reasoning API
  slug: databook-reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-reasoning-api-openapi.yml
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
