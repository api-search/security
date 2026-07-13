---
api_key_in: []
api_specs:
- filename: singlestore-data-api-openapi.yml
  format: yaml
  label: SingleStore Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-data-api-openapi.yml
- filename: singlestore-management-api-openapi.yml
  format: yaml
  label: SingleStore Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Singlestore Authentication
name_suffix: Authentication
oauth_flows: []
overview: SingleStore secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SingleStore
provider_slug: singlestore
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using SingleStore database credentials. Provide the username and password as a Base-64 encoded username:password string in the Authorization header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/singlestore-data-api-openapi.yml
  type: http
- description: Bearer token authentication using a JWT token obtained from the SingleStore Cloud Portal.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/singlestore-data-api-openapi.yml
  - openapi/singlestore-management-api-openapi.yml
  type: http
slug: singlestore-authentication
source_filename: singlestore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/singlestore-data-api-openapi.yml, openapi/singlestore-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using SingleStore database credentials. Provide the\n    username and password as a Base-64 encoded username:password string in the Authorization\n    header.\n  sources:\n  - openapi/singlestore-data-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a JWT token obtained from the SingleStore Cloud\n    Portal.\n  sources:\n  - openapi/singlestore-data-api-openapi.yml\n  - openapi/singlestore-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/authentication/singlestore-authentication.yml
summary_line: http · 2 schemes
tags:
- Database
- SQL
- Analytics
- Cloud
- Distributed SQL
---
