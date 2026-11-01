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
name: Codescene Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeScene secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeScene
provider_slug: codescene
scheme_count: 1
schemes:
- description: 'Fill in the value with: Bearer &lt;your_token&gt;'
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/codescene.json
  type: apiKey
slug: codescene-authentication
source_filename: codescene-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/codescene.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Fill in the value with: Bearer &lt;your_token&gt;'\n  sources:\n  - openapi/codescene.json\n"
source_yaml_url: https://artifacts.apis.io/codescene/authentication/codescene-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- Code Analysis
- Technical Debt
- DevOps
---
