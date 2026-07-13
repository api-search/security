---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Language Translator V3
  slug: language-translator-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-translate/refs/heads/main/openapi/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ibm Translate Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM Language Translator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IBM Language Translator
provider_slug: ibm-translate
scheme_count: 1
schemes:
- description: IBM Cloud IAM token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yaml
  type: http
slug: ibm-translate-authentication
source_filename: ibm-translate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: IBM Cloud IAM token authentication\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-translate/refs/heads/main/authentication/ibm-translate-authentication.yml
summary_line: http · 1 scheme
tags:
- Translation
- Natural Language Processing
- Machine Translation
- IBM Watson
- AI
- Text Analysis
- Deprecated
---
