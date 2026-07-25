---
api_key_in: []
api_specs:
- filename: vcv-chatbot-api-openapi.yml
  format: yaml
  label: VCV chatbot API
  slug: vcv-chatbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-chatbot-api-openapi.yml
- filename: vcv-companies-api-openapi.yml
  format: yaml
  label: VCV companies API
  slug: vcv-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-companies-api-openapi.yml
- filename: vcv-countries-api-openapi.yml
  format: yaml
  label: VCV countries API
  slug: vcv-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-countries-api-openapi.yml
- filename: vcv-enumeration-api-openapi.yml
  format: yaml
  label: VCV enumeration API
  slug: vcv-enumeration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-enumeration-api-openapi.yml
- filename: vcv-integration-api-openapi.yml
  format: yaml
  label: VCV integration API
  slug: vcv-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-integration-api-openapi.yml
- filename: vcv-interview-api-openapi.yml
  format: yaml
  label: VCV interview API
  slug: vcv-interview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-interview-api-openapi.yml
- filename: vcv-invite-api-openapi.yml
  format: yaml
  label: VCV invite API
  slug: vcv-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-invite-api-openapi.yml
- filename: vcv-languages-api-openapi.yml
  format: yaml
  label: VCV Languages API
  slug: vcv-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-languages-api-openapi.yml
- filename: vcv-limits-api-openapi.yml
  format: yaml
  label: VCV limits API
  slug: vcv-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-limits-api-openapi.yml
- filename: vcv-response-api-openapi.yml
  format: yaml
  label: VCV response API
  slug: vcv-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-response-api-openapi.yml
- filename: vcv-survey-api-openapi.yml
  format: yaml
  label: VCV survey API
  slug: vcv-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-survey-api-openapi.yml
- filename: vcv-tags-api-openapi.yml
  format: yaml
  label: VCV tags API
  slug: vcv-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-tags-api-openapi.yml
- filename: vcv-test-api-openapi.yml
  format: yaml
  label: VCV test API
  slug: vcv-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-test-api-openapi.yml
- filename: vcv-users-api-openapi.yml
  format: yaml
  label: VCV users API
  slug: vcv-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-users-api-openapi.yml
- filename: vcv-vacancy-api-openapi.yml
  format: yaml
  label: VCV vacancy API
  slug: vcv-vacancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-vacancy-api-openapi.yml
- filename: vcv-videointerview-api-openapi.yml
  format: yaml
  label: VCV videointerview API
  slug: vcv-videointerview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-videointerview-api-openapi.yml
- filename: vcv-webhook-api-openapi.yml
  format: yaml
  label: VCV webhook API
  slug: vcv-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vcv Authentication
name_suffix: Authentication
oauth_flows: []
overview: VCV secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VCV
provider_slug: vcv
scheme_count: 1
schemes:
- bearerFormat: token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vcv-openapi-original.yml
  - openapi/vcv-openapi.yml
  type: http
slug: vcv-authentication
source_filename: vcv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vcv-openapi-original.yml, openapi/vcv-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/vcv-openapi-original.yml\n  - openapi/vcv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/authentication/vcv-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Recruiting
- Human Resources
- Video Interviews
- Talent Acquisition
- Hiring
- Assessments
---
