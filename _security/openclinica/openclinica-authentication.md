---
api_key_in: []
api_specs:
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Authentication API
  slug: openclinica-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Participants API
  slug: openclinica-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Study Events API
  slug: openclinica-study-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Clinical Data API
  slug: openclinica-clinical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica ODM Metadata API
  slug: openclinica-odm-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Bulk Operations API
  slug: openclinica-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openclinica Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenClinica secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenClinica
provider_slug: openclinica
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openclinica-openapi.yml
  type: http
slug: openclinica-authentication
source_filename: openclinica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openclinica-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openclinica-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/authentication/openclinica-authentication.yml
summary_line: http · 1 scheme
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- CDISC ODM
- Healthcare
- Open Source
---
