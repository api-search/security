---
api_key_in: []
api_specs:
- filename: yugabyte-backup-info-api-openapi.yml
  format: yaml
  label: Yugabyte backup-info API
  slug: yugabyte-backup-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-backup-info-api-openapi.yml
- filename: yugabyte-cluster-api-openapi.yml
  format: yaml
  label: Yugabyte cluster API
  slug: yugabyte-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-cluster-api-openapi.yml
- filename: yugabyte-cluster-info-api-openapi.yml
  format: yaml
  label: Yugabyte cluster-info API
  slug: yugabyte-cluster-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-cluster-info-api-openapi.yml
- filename: yugabyte-pitr-info-api-openapi.yml
  format: yaml
  label: Yugabyte pitr-info API
  slug: yugabyte-pitr-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-pitr-info-api-openapi.yml
- filename: yugabyte-restore-info-api-openapi.yml
  format: yaml
  label: Yugabyte restore-info API
  slug: yugabyte-restore-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-restore-info-api-openapi.yml
- filename: yugabyte-voyager-info-api-openapi.yml
  format: yaml
  label: Yugabyte voyager-info API
  slug: yugabyte-voyager-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-voyager-info-api-openapi.yml
- filename: yugabyte-voyager-metrics-api-openapi.yml
  format: yaml
  label: Yugabyte voyager-metrics API
  slug: yugabyte-voyager-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-voyager-metrics-api-openapi.yml
- filename: yugabyte-xcluster-metrics-api-openapi.yml
  format: yaml
  label: Yugabyte Xcluster Metrics API
  slug: yugabyte-xcluster-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-xcluster-metrics-api-openapi.yml
- filename: yugabyte-xcluster-namespace-details-api-openapi.yml
  format: yaml
  label: Yugabyte Xcluster Namespace Details API
  slug: yugabyte-xcluster-namespace-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-xcluster-namespace-details-api-openapi.yml
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
- Database-as-a-Service
- Open-Source
- SQL
- Data
- Infrastructure
---
