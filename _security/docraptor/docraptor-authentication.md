---
api_key_in: []
api_specs:
- filename: docraptor-openapi.yml
  format: yaml
  label: DocRaptor REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docraptor/refs/heads/main/openapi/docraptor-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docraptor Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocRaptor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DocRaptor
provider_slug: docraptor
scheme_count: 1
schemes:
- description: API key as username, no password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/docraptor-openapi.yml
  type: http
slug: docraptor-authentication
source_filename: docraptor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docraptor-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API key as username, no password\n  sources:\n  - openapi/docraptor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docraptor/refs/heads/main/authentication/docraptor-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Generation
- PDF
- HTML
- Excel
- API
- Prince
---
