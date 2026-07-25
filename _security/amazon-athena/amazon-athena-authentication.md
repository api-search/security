---
api_key_in:
- header
api_specs:
- filename: amazon-athena-data-catalogs-api-openapi.yml
  format: yaml
  label: Amazon Athena Data Catalogs API
  slug: amazon-athena-data-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-data-catalogs-api-openapi.yml
- filename: amazon-athena-databases-api-openapi.yml
  format: yaml
  label: Amazon Athena Databases API
  slug: amazon-athena-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-databases-api-openapi.yml
- filename: amazon-athena-named-queries-api-openapi.yml
  format: yaml
  label: Amazon Athena Named Queries API
  slug: amazon-athena-named-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-named-queries-api-openapi.yml
- filename: amazon-athena-prepared-statements-api-openapi.yml
  format: yaml
  label: Amazon Athena Prepared Statements API
  slug: amazon-athena-prepared-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-prepared-statements-api-openapi.yml
- filename: amazon-athena-query-executions-api-openapi.yml
  format: yaml
  label: Amazon Athena Query Executions API
  slug: amazon-athena-query-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-query-executions-api-openapi.yml
- filename: amazon-athena-table-metadata-api-openapi.yml
  format: yaml
  label: Amazon Athena Table Metadata API
  slug: amazon-athena-table-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-table-metadata-api-openapi.yml
- filename: amazon-athena-tags-api-openapi.yml
  format: yaml
  label: Amazon Athena Tags API
  slug: amazon-athena-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-tags-api-openapi.yml
- filename: amazon-athena-work-groups-api-openapi.yml
  format: yaml
  label: Amazon Athena Work Groups API
  slug: amazon-athena-work-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/openapi/amazon-athena-work-groups-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Athena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Athena secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Athena
provider_slug: amazon-athena
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-athena-openapi.yml
  type: apiKey
slug: amazon-athena-authentication
source_filename: amazon-athena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-athena-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-athena-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-athena/refs/heads/main/authentication/amazon-athena-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Athena
- SQL
- Analytics
- Serverless
---
