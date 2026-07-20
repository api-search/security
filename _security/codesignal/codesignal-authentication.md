---
api_key_in: []
api_specs:
- filename: codesignal-learn-openapi.json
  format: json
  label: CodeSignal Learn Public API
  slug: codesignal-learn-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesignal/refs/heads/main/openapi/codesignal-learn-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Codesignal Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Codesignal secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Codesignal
provider_slug: codesignal
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://codesignal.com/learn/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/codesignal-learn-openapi.json
  type: oauth2
slug: codesignal-authentication
source_filename: codesignal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/codesignal-learn-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://codesignal.com/learn/api/v1/oauth/token\n    scopes: 1\n  sources:\n  - openapi/codesignal-learn-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesignal/refs/heads/main/authentication/codesignal-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Technical Interview
- Skills Assessment
- Hiring
- Recruiting
- Developer Skills
- Assessment
- Education
- GraphQL
- Webhooks
---
