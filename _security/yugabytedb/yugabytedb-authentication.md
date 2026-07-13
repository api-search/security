---
api_key_in:
- header
api_specs:
- filename: yugabytedb-aeon-openapi.yml
  format: yaml
  label: YugabyteDB Aeon REST API
  slug: aeon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/openapi/yugabytedb-aeon-openapi.yml
- filename: yugabytedb-anywhere-v1-universes.yaml
  format: yaml
  label: YugabyteDB Anywhere REST API
  slug: anywhere
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/openapi/yugabytedb-anywhere-v1-universes.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yugabytedb Authentication
name_suffix: Authentication
oauth_flows: []
overview: YugabyteDB secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: YugabyteDB
provider_slug: yugabytedb
scheme_count: 2
schemes:
- description: API key obtained from the YugabyteDB Aeon UI under User Profile > API Keys. Pass the key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/yugabytedb-aeon-openapi.yml
  type: http
- description: API token passed as header
  in: header
  name: apiKeyAuth
  parameter: X-AUTH-YW-API-TOKEN
  sources:
  - openapi/yugabytedb-anywhere-v1-alerts-monitoring.yaml
  - openapi/yugabytedb-anywhere-v1-backups-restore.yaml
  - openapi/yugabytedb-anywhere-v1-full.yaml
  - openapi/yugabytedb-anywhere-v1-high-availability.yaml
  - openapi/yugabytedb-anywhere-v1-providers-infra.yaml
  - openapi/yugabytedb-anywhere-v1-releases-maintenance.yaml
  - openapi/yugabytedb-anywhere-v1-universes.yaml
  - openapi/yugabytedb-anywhere-v1-users-rbac.yaml
  - openapi/yugabytedb-anywhere-v2-openapi.yaml
  type: apiKey
slug: yugabytedb-authentication
source_filename: yugabytedb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yugabytedb-aeon-openapi.yml, openapi/yugabytedb-anywhere-v1-alerts-monitoring.yaml,\n  openapi/yugabytedb-anywhere-v1-backups-restore.yaml, openapi/yugabytedb-anywhere-v1-full.yaml,\n  openapi/yugabytedb-anywhere-v1-high-availability.yaml, openapi/yugabytedb-anywhere-v1-providers-infra.yaml,\n  openapi/yugabytedb-anywhere-v1-releases-maintenance.yaml, openapi/yugabytedb-anywhere-v1-universes.yaml,\n  openapi/yugabytedb-anywhere-v1-users-rbac.yaml, openapi/yugabytedb-anywhere-v2-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key obtained from the YugabyteDB Aeon UI under User Profile > API Keys. Pass\n    the key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/yugabytedb-aeon-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-AUTH-YW-API-TOKEN\n  description:\
  \ API token passed as header\n  sources:\n  - openapi/yugabytedb-anywhere-v1-alerts-monitoring.yaml\n  - openapi/yugabytedb-anywhere-v1-backups-restore.yaml\n  - openapi/yugabytedb-anywhere-v1-full.yaml\n  - openapi/yugabytedb-anywhere-v1-high-availability.yaml\n  - openapi/yugabytedb-anywhere-v1-providers-infra.yaml\n  - openapi/yugabytedb-anywhere-v1-releases-maintenance.yaml\n  - openapi/yugabytedb-anywhere-v1-universes.yaml\n  - openapi/yugabytedb-anywhere-v1-users-rbac.yaml\n  - openapi/yugabytedb-anywhere-v2-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/authentication/yugabytedb-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cloud Database
- Database
- DBaaS
- Distributed SQL
- PostgreSQL
---
