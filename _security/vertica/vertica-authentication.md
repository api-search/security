---
api_key_in: []
api_specs:
- filename: nma_swagger.json
  format: json
  label: Vertica Node Management Agent API
  slug: node-management-agent-api
  spec_type: OpenAPI
  url: https://<node-host>:5554/api-docs/nma_swagger.json
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Vertica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vertica secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vertica
provider_slug: vertica
scheme_count: 1
schemes:
- description: Mutual TLS using NMA client/server certificates
  name: mtls
  sources:
  - openapi/vertica-openapi.yml
  type: mutualTLS
slug: vertica-authentication
source_filename: vertica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vertica-openapi.yml\nsummary:\n  types:\n  - mutualTLS\nschemes:\n- name: mtls\n  type: mutualTLS\n  description: Mutual TLS using NMA client/server certificates\n  sources:\n  - openapi/vertica-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertica/refs/heads/main/authentication/vertica-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Database
- Analytics Database
- Data Warehouse
- Data Lakehouse
- Columnar Database
- MPP
- In-Database Machine Learning
- SQL
---
