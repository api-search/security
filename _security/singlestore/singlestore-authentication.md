---
api_key_in: []
api_specs:
- filename: singlestore-files-api-openapi.yml
  format: yaml
  label: SingleStore Files API
  slug: singlestore-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-files-api-openapi.yml
- filename: singlestore-health-api-openapi.yml
  format: yaml
  label: SingleStore Health API
  slug: singlestore-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-health-api-openapi.yml
- filename: singlestore-jobs-api-openapi.yml
  format: yaml
  label: SingleStore Jobs API
  slug: singlestore-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-jobs-api-openapi.yml
- filename: singlestore-organizations-api-openapi.yml
  format: yaml
  label: SingleStore Organizations API
  slug: singlestore-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-organizations-api-openapi.yml
- filename: singlestore-queries-api-openapi.yml
  format: yaml
  label: SingleStore Queries API
  slug: singlestore-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-queries-api-openapi.yml
- filename: singlestore-regions-api-openapi.yml
  format: yaml
  label: SingleStore Regions API
  slug: singlestore-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-regions-api-openapi.yml
- filename: singlestore-secrets-api-openapi.yml
  format: yaml
  label: SingleStore Secrets API
  slug: singlestore-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-secrets-api-openapi.yml
- filename: singlestore-workspacegroups-api-openapi.yml
  format: yaml
  label: SingleStore WorkspaceGroups API
  slug: singlestore-workspacegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-workspacegroups-api-openapi.yml
- filename: singlestore-workspaces-api-openapi.yml
  format: yaml
  label: SingleStore Workspaces API
  slug: singlestore-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlestore/refs/heads/main/openapi/singlestore-workspaces-api-openapi.yml
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
