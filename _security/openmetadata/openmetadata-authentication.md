---
api_key_in: []
api_specs:
- filename: api-reference
  format: yaml
  label: OpenMetadata REST API
  slug: openmetadata-rest-api
  spec_type: OpenAPI
  url: https://docs.open-metadata.org/api-reference
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openmetadata Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMetadata secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenMetadata
provider_slug: openmetadata
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openmetadata-openmetadata-rest-api-openapi.yml
  type: http
slug: openmetadata-authentication
source_filename: openmetadata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openmetadata-openmetadata-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openmetadata-openmetadata-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmetadata/refs/heads/main/authentication/openmetadata-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Catalog
- Metadata
- Data Governance
- Data Lineage
- Data Quality
- Open Source
- Data Discovery
- Data Observability
---
