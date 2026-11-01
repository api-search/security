---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mintpdf Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: mintpdf-dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mintpdf-dev
provider_slug: mintpdf-dev
scheme_count: 1
schemes:
- description: Your API key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mintpdf-dev-openapi.yml
  type: http
slug: mintpdf-dev-authentication
source_filename: mintpdf-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/mintpdf-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Your API key\n  sources:\n  - openapi/mintpdf-dev-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mintpdf-dev/authentication/mintpdf-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- API
- PDF
- Markdown
- HTML
---
