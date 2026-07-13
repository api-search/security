---
api_key_in: []
api_specs:
- filename: teradata-querygrid-manager-api.yaml
  format: yaml
  label: Teradata QueryGrid Manager API
  slug: querygrid-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-querygrid-manager-api.yaml
- filename: teradata-query-service-api.yaml
  format: yaml
  label: Teradata Query Service API
  slug: query-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-query-service-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teradata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teradata secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teradata
provider_slug: teradata
scheme_count: 1
schemes:
- description: HTTP Basic authentication with Vantage credentials.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/teradata-query-service-api.yaml
  - openapi/teradata-querygrid-manager-api.yaml
  type: http
slug: teradata-authentication
source_filename: teradata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teradata-query-service-api.yaml, openapi/teradata-querygrid-manager-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with Vantage credentials.\n  sources:\n  - openapi/teradata-query-service-api.yaml\n  - openapi/teradata-querygrid-manager-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/authentication/teradata-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
- Fortune 1000
---
