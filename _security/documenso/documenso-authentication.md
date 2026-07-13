---
api_key_in:
- header
api_specs:
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Recipients API
  slug: recipients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Fields API
  slug: fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
- filename: documenso-openapi.yml
  format: yaml
  label: Documenso Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/openapi/documenso-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Documenso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Documenso secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Documenso
provider_slug: documenso
scheme_count: 1
schemes:
- description: API token issued from the Documenso dashboard, sent in the Authorization header (format `api_xxxxxxxx`).
  in: header
  name: apiToken
  parameter: Authorization
  sources:
  - openapi/documenso-openapi.yml
  type: apiKey
slug: documenso-authentication
source_filename: documenso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/documenso-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token issued from the Documenso dashboard, sent in the Authorization header\n    (format `api_xxxxxxxx`).\n  sources:\n  - openapi/documenso-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/documenso/refs/heads/main/authentication/documenso-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Signature
- Documents
- Signing
- Open Source
- DocuSign Alternative
---
