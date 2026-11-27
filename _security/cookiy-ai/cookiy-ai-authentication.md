---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: cookiy-ai-quant-surveys-api-openapi.yml
  format: yaml
  label: Cookiy AI Quant Surveys API
  slug: cookiy-ai-quant-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-quant-surveys-api-openapi.yml
- filename: cookiy-ai-studies-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies API
  slug: cookiy-ai-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-api-openapi.yml
- filename: cookiy-ai-studies-checkout-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies / Checkout API
  slug: cookiy-ai-studies-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-checkout-api-openapi.yml
- filename: cookiy-ai-studies-discussion-guide-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies / Discussion Guide API
  slug: cookiy-ai-studies-discussion-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-discussion-guide-api-openapi.yml
- filename: cookiy-ai-studies-interviews-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies / Interviews API
  slug: cookiy-ai-studies-interviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-interviews-api-openapi.yml
- filename: cookiy-ai-studies-recruit-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies / Recruit API
  slug: cookiy-ai-studies-recruit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-recruit-api-openapi.yml
- filename: cookiy-ai-studies-report-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies / Report API
  slug: cookiy-ai-studies-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-report-api-openapi.yml
- filename: cookiy-ai-studies-synthetic-interview-api-openapi.yml
  format: yaml
  label: Cookiy AI Studies / Synthetic Interview API
  slug: cookiy-ai-studies-synthetic-interview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-studies-synthetic-interview-api-openapi.yml
- filename: cookiy-ai-user-api-openapi.yml
  format: yaml
  label: Cookiy AI User API
  slug: cookiy-ai-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiy-ai/openapi/cookiy-ai-user-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cookiy AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cookiy AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cookiy AI
provider_slug: cookiy-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/cookiy-ai-openapi.yml
  type: http
- in: cookie
  name: cookie
  parameter: Authentication
  sources:
  - openapi/cookiy-ai-openapi.yml
  type: apiKey
slug: cookiy-ai-authentication
source_filename: cookiy-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/cookiy-ai/user-research-skill/blob/HEAD/references/cookiy/cookiy.md\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cookiy-ai-openapi.yml\n- name: cookie\n  type: apiKey\n  in: cookie\n  parameter: Authentication\n  sources:\n  - openapi/cookiy-ai-openapi.yml\ndocs: https://github.com/cookiy-ai/user-research-skill/blob/HEAD/references/cookiy/cookiy.md\nderived_from: openapi/cookiy-ai-openapi.yml\nflow:\n  note: Access token is obtained through browser sign-in (login URL shown in CLI 401\n    errors, s.cookiy.ai console login) and saved locally with \"cookiy save-token <access_token>\";\n    it is sent as a Bearer JWT. 401 responses may carry login_url.\n"
source_yaml_url: https://artifacts.apis.io/cookiy-ai/authentication/cookiy-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- User Research
- AI Interviews
- Surveys
- Market Research
- Participant Recruitment
- Qualitative Research
- Agent Skills
- AI Agents
---
