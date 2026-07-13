---
api_key_in: []
api_specs:
- filename: tidb-cloud-api-openapi.yml
  format: yaml
  label: TiDB Cloud API
  slug: tidb-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-cloud-api-openapi.yml
- filename: tidb-cloud-data-service-openapi.yml
  format: yaml
  label: TiDB Cloud Data Service API
  slug: tidb-cloud-data-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-cloud-data-service-openapi.yml
- filename: tidb-cloud-chat2query-openapi.yml
  format: yaml
  label: TiDB Cloud Chat2Query API
  slug: tidb-cloud-chat2query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-cloud-chat2query-openapi.yml
- filename: tidb-http-api-openapi.yml
  format: yaml
  label: TiDB HTTP API
  slug: tidb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-http-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tidb Authentication
name_suffix: Authentication
oauth_flows: []
overview: tidb secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: tidb
provider_slug: tidb
scheme_count: 1
schemes:
- description: HTTP Digest Authentication using a TiDB Cloud API public key as the username and private key as the password. Keys are generated in the TiDB Cloud console under Organization Settings > API Keys.
  name: digestAuth
  scheme: digest
  sources:
  - openapi/tidb-cloud-api-openapi.yml
  - openapi/tidb-cloud-chat2query-openapi.yml
  - openapi/tidb-cloud-data-service-openapi.yml
  type: http
slug: tidb-authentication
source_filename: tidb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tidb-cloud-api-openapi.yml, openapi/tidb-cloud-chat2query-openapi.yml, openapi/tidb-cloud-data-service-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: digestAuth\n  type: http\n  scheme: digest\n  description: HTTP Digest Authentication using a TiDB Cloud API public key as the username\n    and private key as the password. Keys are generated in the TiDB Cloud console under Organization\n    Settings > API Keys.\n  sources:\n  - openapi/tidb-cloud-api-openapi.yml\n  - openapi/tidb-cloud-chat2query-openapi.yml\n  - openapi/tidb-cloud-data-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/authentication/tidb-authentication.yml
summary_line: http · 1 scheme
tags: []
---
