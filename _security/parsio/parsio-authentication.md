---
api_key_in:
- header
api_specs:
- filename: parsio-openapi.yml
  format: yaml
  label: Parsio Mailboxes API
  slug: parsio-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/openapi/parsio-openapi.yml
- filename: parsio-openapi.yml
  format: yaml
  label: Parsio Documents API
  slug: parsio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/openapi/parsio-openapi.yml
- filename: parsio-openapi.yml
  format: yaml
  label: Parsio Webhooks API
  slug: parsio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/openapi/parsio-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parsio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parsio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parsio
provider_slug: parsio
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/parsio-openapi.yml
  type: apiKey
slug: parsio-authentication
source_filename: parsio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parsio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/parsio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsio/refs/heads/main/authentication/parsio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Document Parsing
- Email Parsing
- OCR
- Data Extraction
---
