---
api_key_in: []
api_specs:
- filename: bigid-authentication-api-openapi.yml
  format: yaml
  label: BigID Authentication API
  slug: bigid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-authentication-api-openapi.yml
- filename: bigid-data-sources-api-openapi.yml
  format: yaml
  label: BigID Data Sources API
  slug: bigid-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-sources-api-openapi.yml
- filename: bigid-scans-api-openapi.yml
  format: yaml
  label: BigID Scans API
  slug: bigid-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-scans-api-openapi.yml
- filename: bigid-dsar-api-openapi.yml
  format: yaml
  label: BigID DSAR API
  slug: bigid-dsar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-dsar-api-openapi.yml
- filename: bigid-actionable-insights-api-openapi.yml
  format: yaml
  label: BigID Actionable Insights API
  slug: bigid-actionable-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-actionable-insights-api-openapi.yml
- filename: bigid-catalog-api-openapi.yml
  format: yaml
  label: BigID Catalog API
  slug: bigid-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-catalog-api-openapi.yml
- filename: bigid-clusters-api-openapi.yml
  format: yaml
  label: BigID Clusters API
  slug: bigid-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-clusters-api-openapi.yml
- filename: bigid-connector-templates-api-openapi.yml
  format: yaml
  label: BigID Connector Templates API
  slug: bigid-connector-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-connector-templates-api-openapi.yml
- filename: bigid-metadata-export-api-openapi.yml
  format: yaml
  label: BigID Metadata Export API
  slug: bigid-metadata-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-metadata-export-api-openapi.yml
- filename: bigid-scan-profiles-api-openapi.yml
  format: yaml
  label: BigID Scan Profiles API
  slug: bigid-scan-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-scan-profiles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bigid Authentication
name_suffix: Authentication
oauth_flows: []
overview: BigID secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BigID
provider_slug: bigid
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bigid-authentication-api-openapi.yml
  - openapi/bigid-cluster-analysis-api-openapi.yml
  - openapi/bigid-data-catalog-api-openapi.yml
  - openapi/bigid-data-posture-api-openapi.yml
  - openapi/bigid-data-sources-api-openapi.yml
  - openapi/bigid-dsar-api-openapi.yml
  - openapi/bigid-scans-api-openapi.yml
  type: http
slug: bigid-authentication
source_filename: bigid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bigid-authentication-api-openapi.yml, openapi/bigid-cluster-analysis-api-openapi.yml,\n  openapi/bigid-data-catalog-api-openapi.yml, openapi/bigid-data-posture-api-openapi.yml, openapi/bigid-data-sources-api-openapi.yml,\n  openapi/bigid-dsar-api-openapi.yml, openapi/bigid-scans-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/bigid-authentication-api-openapi.yml\n  - openapi/bigid-cluster-analysis-api-openapi.yml\n  - openapi/bigid-data-catalog-api-openapi.yml\n  - openapi/bigid-data-posture-api-openapi.yml\n  - openapi/bigid-data-sources-api-openapi.yml\n  - openapi/bigid-dsar-api-openapi.yml\n  - openapi/bigid-scans-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/authentication/bigid-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Security
- DSPM
- DLP
- Privacy
- AI Security
- Data Catalog
- DSAR
- Data Discovery
- Compliance
---
