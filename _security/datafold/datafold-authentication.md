---
api_key_in:
- header
api_specs:
- filename: datafold-audit-logs-api-openapi.yml
  format: yaml
  label: Datafold Audit Logs API
  slug: datafold-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-audit-logs-api-openapi.yml
- filename: datafold-bi-added-api-openapi.yml
  format: yaml
  label: Datafold bi_added API
  slug: datafold-bi-added-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-added-api-openapi.yml
- filename: datafold-bi-api-openapi.yml
  format: yaml
  label: Datafold BI API
  slug: datafold-bi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-api-openapi.yml
- filename: datafold-bi-deleted-api-openapi.yml
  format: yaml
  label: Datafold bi_deleted API
  slug: datafold-bi-deleted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-deleted-api-openapi.yml
- filename: datafold-bi-modified-api-openapi.yml
  format: yaml
  label: Datafold bi_modified API
  slug: datafold-bi-modified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-modified-api-openapi.yml
- filename: datafold-bolt-api-openapi.yml
  format: yaml
  label: Datafold bolt API
  slug: datafold-bolt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bolt-api-openapi.yml
- filename: datafold-ci-api-openapi.yml
  format: yaml
  label: Datafold CI API
  slug: datafold-ci-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-ci-api-openapi.yml
- filename: datafold-data-diffs-api-openapi.yml
  format: yaml
  label: Datafold Data diffs API
  slug: datafold-data-diffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-data-diffs-api-openapi.yml
- filename: datafold-data-source-added-api-openapi.yml
  format: yaml
  label: Datafold data_source_added API
  slug: datafold-data-source-added-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-data-source-added-api-openapi.yml
- filename: datafold-data-sources-api-openapi.yml
  format: yaml
  label: Datafold Data sources API
  slug: datafold-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-data-sources-api-openapi.yml
- filename: datafold-diff-created-api-openapi.yml
  format: yaml
  label: Datafold diff_created API
  slug: datafold-diff-created-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-diff-created-api-openapi.yml
- filename: datafold-explore-api-openapi.yml
  format: yaml
  label: Datafold Explore API
  slug: datafold-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-explore-api-openapi.yml
- filename: datafold-monitors-api-openapi.yml
  format: yaml
  label: Datafold Monitors API
  slug: datafold-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-monitors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Datafold Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafold secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datafold
provider_slug: datafold
scheme_count: 1
schemes:
- description: Use the 'Authorization' header with the format 'Key <api-key>'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/datafold-openapi.json
  type: apiKey
slug: datafold-authentication
source_filename: datafold-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datafold-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Use the 'Authorization' header with the format 'Key <api-key>'\n  sources:\n  - openapi/datafold-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/authentication/datafold-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Reliability
- Data Diff
- Data Quality
- Column-Level Lineage
- Data Pipeline
- CI/CD Integration
- Anomaly Detection
- Data Observability
- Data Migrations
---
