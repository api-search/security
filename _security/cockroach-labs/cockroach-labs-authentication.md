---
api_key_in:
- header
api_specs:
- filename: cockroach-labs-cloud-api-openapi.yml
  format: yaml
  label: CockroachDB Cloud API
  slug: cockroach-labs-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cockroach-labs/refs/heads/main/openapi/cockroach-labs-cloud-api-openapi.yml
- filename: cockroach-labs-cluster-api-openapi.yml
  format: yaml
  label: CockroachDB Cluster API
  slug: cockroach-labs-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cockroach-labs/refs/heads/main/openapi/cockroach-labs-cluster-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cockroach Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cockroach Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cockroach Labs
provider_slug: cockroach-labs
scheme_count: 2
schemes:
- description: Bearer token authentication. Generate a token in the CockroachDB Cloud Console under Organization Settings > API Access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cockroach-labs-cloud-api-openapi.yml
  type: http
- description: Session token obtained from the /api/v2/login/ endpoint. Include this header with all authenticated requests.
  in: header
  name: sessionAuth
  parameter: X-Cockroach-API-Session
  sources:
  - openapi/cockroach-labs-cluster-api-openapi.yml
  type: apiKey
slug: cockroach-labs-authentication
source_filename: cockroach-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cockroach-labs-cloud-api-openapi.yml, openapi/cockroach-labs-cluster-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Generate a token in the CockroachDB Cloud Console\n    under Organization Settings > API Access.\n  sources:\n  - openapi/cockroach-labs-cloud-api-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: X-Cockroach-API-Session\n  description: Session token obtained from the /api/v2/login/ endpoint. Include this header\n    with all authenticated requests.\n  sources:\n  - openapi/cockroach-labs-cluster-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cockroach-labs/refs/heads/main/authentication/cockroach-labs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cluster Management
- Cloud
- Database
- Distributed SQL
- Infrastructure
- PostgreSQL Compatible
- SQL
---
