---
api_key_in: []
api_specs:
- filename: oracle-goldengate-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate REST API
  slug: oracle-goldengate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-rest-api-openapi.yml
- filename: oracle-goldengate-big-data-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate for Big Data REST API
  slug: oracle-goldengate-for-big-data-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-big-data-rest-api-openapi.yml
- filename: oracle-goldengate-veridata-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Veridata REST API
  slug: oracle-goldengate-veridata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-veridata-rest-api-openapi.yml
- filename: oracle-goldengate-cloud-service-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Cloud Service API
  slug: oracle-goldengate-cloud-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-cloud-service-api-openapi.yml
- filename: oracle-goldengate-stream-analytics-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Stream Analytics REST API
  slug: oracle-goldengate-stream-analytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml
- filename: oracle-goldengate-data-streams-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Data Streams REST API
  slug: oracle-goldengate-data-streams-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-data-streams-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Goldengate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle GoldenGate secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-goldengate-big-data-rest-api-openapi.yml
  - openapi/oracle-goldengate-data-streams-rest-api-openapi.yml
  - openapi/oracle-goldengate-rest-api-openapi.yml
  - openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml
  - openapi/oracle-goldengate-veridata-rest-api-openapi.yml
  type: http
- description: OCI API request signature (RFC 7616) or bearer token authentication
  name: ociSignature
  scheme: bearer
  sources:
  - openapi/oracle-goldengate-cloud-service-api-openapi.yml
  type: http
slug: oracle-goldengate-authentication
source_filename: oracle-goldengate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-goldengate-big-data-rest-api-openapi.yml, openapi/oracle-goldengate-cloud-service-api-openapi.yml,\n  openapi/oracle-goldengate-data-streams-rest-api-openapi.yml, openapi/oracle-goldengate-rest-api-openapi.yml,\n  openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml, openapi/oracle-goldengate-veridata-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/oracle-goldengate-big-data-rest-api-openapi.yml\n  - openapi/oracle-goldengate-data-streams-rest-api-openapi.yml\n  - openapi/oracle-goldengate-rest-api-openapi.yml\n  - openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml\n  - openapi/oracle-goldengate-veridata-rest-api-openapi.yml\n- name: ociSignature\n  type: http\n  scheme: bearer\n  description: OCI API request signature (RFC 7616) or bearer token authentication\n  sources:\n  - openapi/oracle-goldengate-cloud-service-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/authentication/oracle-goldengate-authentication.yml
summary_line: http · 2 schemes
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
---
