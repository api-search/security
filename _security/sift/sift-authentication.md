---
api_key_in: []
api_specs:
- filename: sift-openapi.yml
  format: yaml
  label: Sift Events API
  slug: sift-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Score API
  slug: sift-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Decisions API
  slug: sift-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Workflow Status API
  slug: sift-workflow-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Labels API
  slug: sift-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Verification API
  slug: sift-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift PSP Merchant Management API
  slug: sift-psp-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sift
provider_slug: sift
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication using your Sift REST API key as the username and an empty password (Authorization: Basic base64(api_key + ":")). The ingestion APIs (Events, Score, Labels) also accept the key as `$api_key` in the JSON request body. Account-scoped APIs (Decisions, Workflows, PSP Merchant Management) additionally require your numeric Account ID in the URL path. Mobile SDKs authenticate separately with a Beacon Key. There is no OAuth.'
  name: apiKeyBasic
  scheme: basic
  sources:
  - openapi/sift-openapi.yml
  - https://developers.sift.com/docs/curl/apis-overview
  type: http
slug: sift-authentication
source_filename: sift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/sift-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyBasic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using your Sift REST API key as the username and an\n    empty password (Authorization: Basic base64(api_key + \":\")). The ingestion\n    APIs (Events, Score, Labels) also accept the key as `$api_key` in the JSON\n    request body. Account-scoped APIs (Decisions, Workflows, PSP Merchant\n    Management) additionally require your numeric Account ID in the URL path.\n    Mobile SDKs authenticate separately with a Beacon Key. There is no OAuth.\n  sources:\n  - openapi/sift-openapi.yml\n  - https://developers.sift.com/docs/curl/apis-overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/authentication/sift-authentication.yml
summary_line: http · 1 scheme
tags:
- Fraud Detection
- Fraud Prevention
- Risk
- Trust and Safety
- Machine Learning
- Payment Fraud
- Account Takeover
- Chargebacks
- Digital Trust
---
