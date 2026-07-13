---
api_key_in:
- header
api_specs:
- filename: dolthub-openapi.yml
  format: yaml
  label: DoltHub SQL Query API
  slug: dolthub-sql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/openapi/dolthub-openapi.yml
- filename: dolthub-openapi.yml
  format: yaml
  label: DoltHub Write API
  slug: dolthub-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/openapi/dolthub-openapi.yml
- filename: dolthub-openapi.yml
  format: yaml
  label: DoltHub Repositories and Branches API
  slug: dolthub-repositories-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/openapi/dolthub-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dolthub Authentication
name_suffix: Authentication
oauth_flows: []
overview: DoltHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DoltHub
provider_slug: dolthub
scheme_count: 1
schemes:
- description: DoltHub API token sent as the `authorization` header in the form "token YOUR_API_TOKEN". Required for write queries and access to private databases.
  in: header
  name: tokenAuth
  parameter: authorization
  sources:
  - openapi/dolthub-openapi.yml
  type: apiKey
slug: dolthub-authentication
source_filename: dolthub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dolthub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: DoltHub API token sent as the `authorization` header in the form \"token YOUR_API_TOKEN\".\n    Required for write queries and access to private databases.\n  sources:\n  - openapi/dolthub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/authentication/dolthub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Database
- SQL
- Version Control
- Git for Data
- MySQL
---
