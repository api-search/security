---
api_key_in:
- header
api_specs:
- filename: typesense-analytics-events-api-openapi.yml
  format: yaml
  label: Typesense Analytics Events API
  slug: typesense-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-analytics-events-api-openapi.yml
- filename: typesense-analytics-operations-api-openapi.yml
  format: yaml
  label: Typesense Analytics Operations API
  slug: typesense-analytics-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-analytics-operations-api-openapi.yml
- filename: typesense-analytics-rules-api-openapi.yml
  format: yaml
  label: Typesense Analytics Rules API
  slug: typesense-analytics-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-analytics-rules-api-openapi.yml
- filename: typesense-cluster-management-api-openapi.yml
  format: yaml
  label: Typesense Cluster Management API
  slug: typesense-cluster-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-cluster-management-api-openapi.yml
- filename: typesense-configuration-changes-api-openapi.yml
  format: yaml
  label: Typesense Configuration Changes API
  slug: typesense-configuration-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-configuration-changes-api-openapi.yml
- filename: typesense-server-configuration-parameters-api-openapi.yml
  format: yaml
  label: Typesense Server Configuration Parameters API
  slug: typesense-server-configuration-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-server-configuration-parameters-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Typesense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Typesense secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Typesense
provider_slug: typesense
scheme_count: 2
schemes:
- description: API key for authenticating requests to the Typesense server.
  in: header
  name: api_key_header
  parameter: X-TYPESENSE-API-KEY
  sources:
  - openapi/typesense-analytics-api-openapi.yml
  - openapi/typesense-conversational-search-api-openapi.yml
  - openapi/typesense-search-api-openapi.yml
  - openapi/typesense-vector-search-api-openapi.yml
  type: apiKey
- description: Cloud management API key for authenticating requests to the Typesense Cloud Management API.
  in: header
  name: cloudApiKey
  parameter: X-TYPESENSE-CLOUD-MANAGEMENT-API-KEY
  sources:
  - openapi/typesense-cloud-management-api-openapi.yml
  type: apiKey
slug: typesense-authentication
source_filename: typesense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/typesense-analytics-api-openapi.yml, openapi/typesense-cloud-management-api-openapi.yml,\n  openapi/typesense-conversational-search-api-openapi.yml, openapi/typesense-search-api-openapi.yml,\n  openapi/typesense-vector-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key_header\n  type: apiKey\n  in: header\n  parameter: X-TYPESENSE-API-KEY\n  description: API key for authenticating requests to the Typesense server.\n  sources:\n  - openapi/typesense-analytics-api-openapi.yml\n  - openapi/typesense-conversational-search-api-openapi.yml\n  - openapi/typesense-search-api-openapi.yml\n  - openapi/typesense-vector-search-api-openapi.yml\n- name: cloudApiKey\n  type: apiKey\n  in: header\n  parameter: X-TYPESENSE-CLOUD-MANAGEMENT-API-KEY\n  description: Cloud management API key for authenticating requests to the Typesense Cloud Management\n    API.\n  sources:\n  - openapi/typesense-cloud-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/authentication/typesense-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Full-Text Search
- Open-Source
- Search Engines
- Typo Tolerance
- Vector Search
---
