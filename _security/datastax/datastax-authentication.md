---
api_key_in: []
api_specs:
- filename: datastax-devops-openapi.json
  format: json
  label: Astra DevOps API
  slug: astra-devops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-devops-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datastax Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataStax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataStax
provider_slug: datastax
scheme_count: 1
schemes:
- description: An application token must be passed in header in order to access the API. https://docs.datastax.com/en/astra-db-serverless/administration/manage-application-tokens.html
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/datastax-devops-openapi.json
  type: http
slug: datastax-authentication
source_filename: datastax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/datastax-devops-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: An application token must be passed in header in order to access the API. https://docs.datastax.com/en/astra-db-serverless/administration/manage-application-tokens.html\n  sources:\n  - openapi/datastax-devops-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/authentication/datastax-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Database
- Vector Database
- Cassandra
- Artificial Intelligence
- RAG
- Serverless
- Streaming
- Developer Tools
---
