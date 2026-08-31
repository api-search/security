---
api_key_in:
- header
api_specs:
- filename: snappt-account-api-openapi.yml
  format: yaml
  label: Snappt Account API
  slug: snappt-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-account-api-openapi.yml
- filename: snappt-applicant-sessions-api-openapi.yml
  format: yaml
  label: Snappt Applicant Sessions API
  slug: snappt-applicant-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-applicant-sessions-api-openapi.yml
- filename: snappt-applicants-api-openapi.yml
  format: yaml
  label: Snappt Applicants API
  slug: snappt-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-applicants-api-openapi.yml
- filename: snappt-id-verification-api-openapi.yml
  format: yaml
  label: Snappt ID Verification API
  slug: snappt-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-id-verification-api-openapi.yml
- filename: snappt-internal-idv-api-openapi.yml
  format: yaml
  label: Snappt Internal IDV API
  slug: snappt-internal-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-internal-idv-api-openapi.yml
- filename: snappt-properties-api-openapi.yml
  format: yaml
  label: Snappt Properties API
  slug: snappt-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-properties-api-openapi.yml
- filename: snappt-webhooks-api-openapi.yml
  format: yaml
  label: Snappt Webhooks API
  slug: snappt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/openapi/snappt-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snappt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snappt secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Snappt
provider_slug: snappt
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snappt-enterprise-api-openapi-original.yml
  type: http
- description: Pass the session token obtained from POST /session
  in: header
  name: snapptSessionAuth
  parameter: x-unauthenticated-session-token
  sources:
  - openapi/snappt-enterprise-api-openapi-original.yml
  type: apiKey
slug: snappt-authentication
source_filename: snappt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/snappt-enterprise-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/snappt-enterprise-api-openapi-original.yml\n- name: snapptSessionAuth\n  type: apiKey\n  in: header\n  parameter: x-unauthenticated-session-token\n  description: Pass the session token obtained from POST /session\n  sources:\n  - openapi/snappt-enterprise-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snappt/refs/heads/main/authentication/snappt-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- fraud-detection
- document-verification
- Identity Verification
- income-verification
- property-management
- multifamily
- real-estate
- proptech
- tenant-screening
- rental-applications
- Webhook
---
