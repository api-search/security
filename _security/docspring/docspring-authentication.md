---
api_key_in: []
api_specs:
- filename: docspring-authentication-api-openapi.yml
  format: yaml
  label: DocSpring Authentication API
  slug: docspring-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-authentication-api-openapi.yml
- filename: docspring-combine-pdfs-api-openapi.yml
  format: yaml
  label: DocSpring Combine PDFs API
  slug: docspring-combine-pdfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-combine-pdfs-api-openapi.yml
- filename: docspring-custom-files-api-openapi.yml
  format: yaml
  label: DocSpring Custom Files API
  slug: docspring-custom-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-custom-files-api-openapi.yml
- filename: docspring-data-requests-api-openapi.yml
  format: yaml
  label: DocSpring Data Requests API
  slug: docspring-data-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-data-requests-api-openapi.yml
- filename: docspring-folders-api-openapi.yml
  format: yaml
  label: DocSpring Folders API
  slug: docspring-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-folders-api-openapi.yml
- filename: docspring-pdf-submissions-api-openapi.yml
  format: yaml
  label: DocSpring PDF Submissions API
  slug: docspring-pdf-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-pdf-submissions-api-openapi.yml
- filename: docspring-submission-batches-api-openapi.yml
  format: yaml
  label: DocSpring Submission Batches API
  slug: docspring-submission-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-submission-batches-api-openapi.yml
- filename: docspring-templates-api-openapi.yml
  format: yaml
  label: DocSpring Templates API
  slug: docspring-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/openapi/docspring-templates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docspring Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocSpring secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DocSpring
provider_slug: docspring
scheme_count: 1
schemes:
- description: 'Username: API Token ID, Password: API Token Secret'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/docspring-docspring-api-openapi.yml
  type: http
slug: docspring-authentication
source_filename: docspring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docspring-docspring-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Username: API Token ID, Password: API Token Secret'\n  sources:\n  - openapi/docspring-docspring-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/authentication/docspring-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- Document Generation
- PDF Templates
- E-Signatures
- Forms
- HTML to PDF
- Document Automation
---
