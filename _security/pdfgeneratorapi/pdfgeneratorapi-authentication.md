---
api_key_in: []
api_specs:
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Templates API
  slug: pdfgeneratorapi-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Documents / Generate API
  slug: pdfgeneratorapi-documents-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Workspaces API
  slug: pdfgeneratorapi-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Data Fields API
  slug: pdfgeneratorapi-data-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pdfgeneratorapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: PDF Generator API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PDF Generator API
provider_slug: pdfgeneratorapi
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Short-lived JSON Web Token signed with HS256 using your API secret. Claims: iss (API key), sub (workspace identifier), exp (expiration).'
  name: JWT
  scheme: bearer
  sources:
  - openapi/pdfgeneratorapi-openapi.yml
  type: http
slug: pdfgeneratorapi-authentication
source_filename: pdfgeneratorapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdfgeneratorapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Short-lived JSON Web Token signed with HS256 using your API secret. Claims:\n    iss (API key), sub (workspace identifier), exp (expiration).'\n  sources:\n  - openapi/pdfgeneratorapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/authentication/pdfgeneratorapi-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- Document Generation
- Templates
- Reporting
- Workspaces
---
