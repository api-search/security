---
api_key_in:
- header
api_specs:
- filename: docuseal-docuseal-api-openapi.yml
  format: yaml
  label: DocuSeal REST API
  slug: docuseal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/openapi/docuseal-docuseal-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Docuseal Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocuSeal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DocuSeal
provider_slug: docuseal
scheme_count: 1
schemes:
- in: header
  name: AuthToken
  parameter: X-Auth-Token
  sources:
  - openapi/docuseal-docuseal-api-openapi.yml
  type: apiKey
slug: docuseal-authentication
source_filename: docuseal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docuseal-docuseal-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/docuseal-docuseal-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docuseal/refs/heads/main/authentication/docuseal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Signing
- eSignature
- Electronic Signature
- Document Management
- PDF
- Templates
- Open Source
- Webhooks
- Embedding
---
