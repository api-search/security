---
api_key_in: []
api_specs:
- filename: teradata-api-info-api-openapi.yml
  format: yaml
  label: Teradata API Info API
  slug: teradata-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-api-info-api-openapi.yml
- filename: teradata-configuration-api-openapi.yml
  format: yaml
  label: Teradata Configuration API
  slug: teradata-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-configuration-api-openapi.yml
- filename: teradata-issues-api-openapi.yml
  format: yaml
  label: Teradata Issues API
  slug: teradata-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-issues-api-openapi.yml
- filename: teradata-managers-api-openapi.yml
  format: yaml
  label: Teradata Managers API
  slug: teradata-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-managers-api-openapi.yml
- filename: teradata-nodes-api-openapi.yml
  format: yaml
  label: Teradata Nodes API
  slug: teradata-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-nodes-api-openapi.yml
- filename: teradata-operations-api-openapi.yml
  format: yaml
  label: Teradata Operations API
  slug: teradata-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-operations-api-openapi.yml
- filename: teradata-queries-api-openapi.yml
  format: yaml
  label: Teradata Queries API
  slug: teradata-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-queries-api-openapi.yml
- filename: teradata-sessions-api-openapi.yml
  format: yaml
  label: Teradata Sessions API
  slug: teradata-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-sessions-api-openapi.yml
- filename: teradata-software-api-openapi.yml
  format: yaml
  label: Teradata Software API
  slug: teradata-software-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-software-api-openapi.yml
- filename: teradata-systems-api-openapi.yml
  format: yaml
  label: Teradata Systems API
  slug: teradata-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-systems-api-openapi.yml
- filename: teradata-users-api-openapi.yml
  format: yaml
  label: Teradata Users API
  slug: teradata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-users-api-openapi.yml
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
- Machine-Learning
- SQL
- Fortune 1000
---
