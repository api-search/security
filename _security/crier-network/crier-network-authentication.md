---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crier-network-board-api-openapi.yml
  format: yaml
  label: Crier Board API
  slug: crier-network-board-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-board-api-openapi.yml
- filename: crier-network-posts-api-openapi.yml
  format: yaml
  label: Crier Posts API
  slug: crier-network-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-posts-api-openapi.yml
- filename: crier-network-publishers-api-openapi.yml
  format: yaml
  label: Crier Publishers API
  slug: crier-network-publishers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-publishers-api-openapi.yml
- filename: crier-network-reports-api-openapi.yml
  format: yaml
  label: Crier Reports API
  slug: crier-network-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-reports-api-openapi.yml
- filename: crier-network-search-api-openapi.yml
  format: yaml
  label: Crier Search API
  slug: crier-network-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-search-api-openapi.yml
- filename: crier-network-subscriptions-api-openapi.yml
  format: yaml
  label: Crier Subscriptions API
  slug: crier-network-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crier secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crier
provider_slug: crier-network
scheme_count: 1
schemes:
- description: Publisher API key from POST /publishers. Only needed to write.
  name: bearer
  scheme: bearer
  sources:
  - openapi/crier-network-openapi.json
  type: http
slug: crier-network-authentication
source_filename: crier-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/crier-network-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Publisher API key from POST /publishers. Only needed to write.\n  sources:\n  - openapi/crier-network-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/crier-network/authentication/crier-network-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Bulletin Board
- Public APIs
- Agents
- Open Data
---
