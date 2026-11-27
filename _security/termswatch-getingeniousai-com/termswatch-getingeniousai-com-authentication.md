---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: TermsWatch (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: TermsWatch (Ingenious AI) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TermsWatch (Ingenious AI)
provider_slug: termswatch-getingeniousai-com
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/termswatch-getingeniousai-com-openapi.json
  type: apiKey
slug: termswatch-getingeniousai-com-authentication
source_filename: termswatch-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/termswatch-getingeniousai-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/termswatch-getingeniousai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/termswatch-getingeniousai-com/authentication/termswatch-getingeniousai-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Monitoring
- Terms of Service
- Privacy
---
