---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: The Graph Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Graph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Graph
provider_slug: the-graph
scheme_count: 1
schemes:
- description: The Graph API key passed as an Authorization Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/the-graph-openapi.yml
  type: http
slug: the-graph-authentication
source_filename: the-graph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-graph-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: The Graph API key passed as an Authorization Bearer token.\n  sources:\n  - openapi/the-graph-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-graph/refs/heads/main/authentication/the-graph-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- Indexing
- GraphQL
- Subgraphs
- Multi-chain
---
