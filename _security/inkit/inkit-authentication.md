---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Inkit Document Generation API
  slug: inkit-document-generation-api
  spec_type: OpenAPI
  url: https://docs.inkit.com/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Inkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inkit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inkit
provider_slug: inkit
scheme_count: 1
schemes:
- description: API token for Inkit authentication
  in: header
  name: ApiKeyAuth
  parameter: X-Inkit-API-Token
  sources:
  - openapi/inkit-document-generation-api-openapi.yml
  type: apiKey
slug: inkit-authentication
source_filename: inkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inkit-document-generation-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Inkit-API-Token\n  description: API token for Inkit authentication\n  sources:\n  - openapi/inkit-document-generation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inkit/refs/heads/main/authentication/inkit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Generation
- PDF
- Templates
- Digital Signatures
- Workflows
- Document Management
- Secure Documents
- Compliance
- HIPAA
- Enterprise
---
