---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: QuizAPI
  slug: quiz-api
  spec_type: OpenAPI
  url: https://quizapi.io/api/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quiz Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuizAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QuizAPI
provider_slug: quiz-api
scheme_count: 1
schemes:
- description: 'Pass your API key as a Bearer token: `Authorization: Bearer [example key]`. Alternatively, use the `api_key` query parameter.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/quiz-api-openapi.json
  type: http
slug: quiz-api-authentication
source_filename: quiz-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quiz-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your API key as a Bearer token: `Authorization: Bearer [example key]`. Alternatively,\n    use the `api_key` query parameter.'\n  sources:\n  - openapi/quiz-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiz-api/refs/heads/main/authentication/quiz-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Quizzes
- Trivia
- Education
- Assessment
- Content
---
