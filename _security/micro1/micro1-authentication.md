---
api_key_in:
- header
api_specs:
- filename: micro1-interview-api-openapi.yml
  format: yaml
  label: micro1 Interview API
  slug: micro1-interview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-interview-api-openapi.yml
- filename: micro1-interview-reports-api-openapi.yml
  format: yaml
  label: micro1 Interview Reports API
  slug: micro1-interview-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-interview-reports-api-openapi.yml
- filename: micro1-invite-candidate-api-openapi.yml
  format: yaml
  label: micro1 Invite Candidate API
  slug: micro1-invite-candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-invite-candidate-api-openapi.yml
- filename: micro1-job-api-openapi.yml
  format: yaml
  label: micro1 Job API
  slug: micro1-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-job-api-openapi.yml
- filename: micro1-job-applicant-api-openapi.yml
  format: yaml
  label: micro1 Job Applicant API
  slug: micro1-job-applicant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-job-applicant-api-openapi.yml
- filename: micro1-webhook-api-openapi.yml
  format: yaml
  label: micro1 Webhook API
  slug: micro1-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Micro1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: micro1 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: micro1
provider_slug: micro1
scheme_count: 1
schemes:
- description: API key to access the API
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/micro1-ai-recruiter-openapi.yml
  type: apiKey
slug: micro1-authentication
source_filename: micro1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/micro1-ai-recruiter-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key to access the API\n  sources:\n  - openapi/micro1-ai-recruiter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/authentication/micro1-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- recruiting
- hiring
- ai-interviews
- talent-assessment
- candidate-screening
- applicant-tracking
- human-resources
- proctoring
- Webhook
- agent-native
- AI Training Data
---
