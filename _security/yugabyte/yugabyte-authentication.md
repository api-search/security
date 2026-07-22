---
api_key_in: []
api_specs:
- filename: yugabyte-yugabyted-openapi-original.yaml
  format: yaml
  label: YugabyteDB yugabyted UI API
  slug: yugabytedb-yugabyted-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-yugabyted-openapi-original.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yugabyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yugabyte secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yugabyte
provider_slug: yugabyte
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuthToken
  scheme: bearer
  sources:
  - openapi/yugabyte-yugabyted-openapi-original.yaml
  type: http
slug: yugabyte-authentication
source_filename: yugabyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/yugabyte-yugabyted-openapi-original.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuthToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/yugabyte-yugabyted-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/authentication/yugabyte-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Database
- Distributed SQL
- PostgreSQL
- Cloud
- DBaaS
- Open Source
- SQL
- Data
- Infrastructure
---
