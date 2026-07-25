---
api_key_in:
- header
api_specs:
- filename: elastic-account-api-openapi.yml
  format: yaml
  label: Elastic Account API
  slug: elastic-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-account-api-openapi.yml
- filename: elastic-cluster-api-openapi.yml
  format: yaml
  label: Elastic Cluster API
  slug: elastic-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-cluster-api-openapi.yml
- filename: elastic-dataviews-api-openapi.yml
  format: yaml
  label: Elastic DataViews API
  slug: elastic-dataviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-dataviews-api-openapi.yml
- filename: elastic-deployments-api-openapi.yml
  format: yaml
  label: Elastic Deployments API
  slug: elastic-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-deployments-api-openapi.yml
- filename: elastic-documents-api-openapi.yml
  format: yaml
  label: Elastic Documents API
  slug: elastic-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-documents-api-openapi.yml
- filename: elastic-indices-api-openapi.yml
  format: yaml
  label: Elastic Indices API
  slug: elastic-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-indices-api-openapi.yml
- filename: elastic-savedobjects-api-openapi.yml
  format: yaml
  label: Elastic SavedObjects API
  slug: elastic-savedobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-savedobjects-api-openapi.yml
- filename: elastic-search-api-openapi.yml
  format: yaml
  label: Elastic Search API
  slug: elastic-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-search-api-openapi.yml
- filename: elastic-security-api-openapi.yml
  format: yaml
  label: Elastic Security API
  slug: elastic-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-security-api-openapi.yml
- filename: elastic-spaces-api-openapi.yml
  format: yaml
  label: Elastic Spaces API
  slug: elastic-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-spaces-api-openapi.yml
- filename: elastic-status-api-openapi.yml
  format: yaml
  label: Elastic Status API
  slug: elastic-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-status-api-openapi.yml
- filename: elastic-trafficfilters-api-openapi.yml
  format: yaml
  label: Elastic TrafficFilters API
  slug: elastic-trafficfilters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-trafficfilters-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elastic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elastic
provider_slug: elastic
scheme_count: 2
schemes:
- description: ApiKey <api_key>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elastic-cloud-openapi.yml
  - openapi/elastic-elasticsearch-openapi.yml
  - openapi/elastic-kibana-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elastic-elasticsearch-openapi.yml
  - openapi/elastic-kibana-openapi.yml
  type: http
slug: elastic-authentication
source_filename: elastic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elastic-cloud-openapi.yml, openapi/elastic-elasticsearch-openapi.yml, openapi/elastic-kibana-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: ApiKey <api_key>\n  sources:\n  - openapi/elastic-cloud-openapi.yml\n  - openapi/elastic-elasticsearch-openapi.yml\n  - openapi/elastic-kibana-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elastic-elasticsearch-openapi.yml\n  - openapi/elastic-kibana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/authentication/elastic-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Search
- Analytics
- Observability
- Security
- Visualization
- Cloud
---
