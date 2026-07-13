---
api_key_in:
- header
api_specs:
- filename: parseur-openapi.yml
  format: yaml
  label: Parseur API
  slug: parseur-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseur/refs/heads/main/openapi/parseur-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parseur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parseur secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parseur
provider_slug: parseur
scheme_count: 1
schemes:
- description: 'Use header: Authorization: Token YOUR_API_KEY. API keys are here: https://app.parseur.com/account/api-keys'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/parseur-openapi.yml
  type: apiKey
slug: parseur-authentication
source_filename: parseur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parseur-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Use header: Authorization: Token YOUR_API_KEY. API keys are here: https://app.parseur.com/account/api-keys'\n  sources:\n  - openapi/parseur-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseur/refs/heads/main/authentication/parseur-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Document Parsing
- Document Processing
- Document Extraction
- Email Parsing
- OCR
- Data Extraction
- Vision AI
- Automation
- Webhooks
- Mailboxes
- SaaS
---
