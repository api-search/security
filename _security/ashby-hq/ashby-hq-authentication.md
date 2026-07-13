---
api_key_in:
- header
api_specs:
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Applications API
  slug: ashby-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Candidates API
  slug: ashby-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Jobs API
  slug: ashby-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Interviews API
  slug: ashby-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Offers API
  slug: ashby-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Approvals API
  slug: ashby-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Surveys & Feedback API
  slug: ashby-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Assessments API
  slug: ashby-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Custom Fields API
  slug: ashby-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Organization API
  slug: ashby-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Files API
  slug: ashby-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Reports API
  slug: ashby-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Webhooks API
  slug: ashby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby API Keys API
  slug: ashby-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ashby Hq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ashby secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ashby
provider_slug: ashby-hq
scheme_count: 2
schemes:
- description: HTTP Basic Auth. Send your Ashby API key as the username and leave the password blank.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/ashby-openapi.yml
  type: http
- description: HMAC-SHA256 signature of the webhook payload, used to verify webhook authenticity.
  in: header
  name: WebhookSignature
  parameter: Ashby-Signature
  sources:
  - openapi/ashby-openapi.yml
  type: apiKey
slug: ashby-hq-authentication
source_filename: ashby-hq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ashby-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth. Send your Ashby API key as the username and leave the password\n    blank.\n  sources:\n  - openapi/ashby-openapi.yml\n- name: WebhookSignature\n  type: apiKey\n  in: header\n  parameter: Ashby-Signature\n  description: HMAC-SHA256 signature of the webhook payload, used to verify webhook authenticity.\n  sources:\n  - openapi/ashby-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/authentication/ashby-hq-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- ATS
- Applicant Tracking System
- Recruiting
- Talent Acquisition
- Sourcing
- CRM
- Scheduling
- Analytics
- Hiring
- HR Tech
- AI
---
