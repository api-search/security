---
api_key_in:
- header
api_specs:
- filename: airmeet-openapi.yml
  format: yaml
  label: Airmeet Public API
  slug: airmeet-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmeet/refs/heads/main/openapi/airmeet-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airmeet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airmeet secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Airmeet
provider_slug: airmeet
scheme_count: 5
schemes:
- description: Community access key, presented at POST /auth.
  in: header
  name: accessKey
  parameter: X-Airmeet-Access-Key
  sources:
  - openapi/airmeet-openapi.yml
  type: apiKey
- description: Community secret key, presented at POST /auth.
  in: header
  name: secretKey
  parameter: X-Airmeet-Secret-Key
  sources:
  - openapi/airmeet-openapi.yml
  type: apiKey
- description: Bearer access token issued by POST /auth, valid for 30 days.
  in: header
  name: accessToken
  parameter: X-Airmeet-Access-Token
  sources:
  - openapi/airmeet-openapi.yml
  type: apiKey
- description: Access key for webhook registration.
  in: header
  name: webhookAccessKey
  parameter: x-access-key
  sources:
  - openapi/airmeet-openapi.yml
  type: apiKey
- description: Secret key for webhook registration.
  in: header
  name: webhookSecretKey
  parameter: x-secret-key
  sources:
  - openapi/airmeet-openapi.yml
  type: apiKey
slug: airmeet-authentication
source_filename: airmeet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/airmeet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessKey\n  type: apiKey\n  in: header\n  parameter: X-Airmeet-Access-Key\n  description: Community access key, presented at POST /auth.\n  sources:\n  - openapi/airmeet-openapi.yml\n- name: secretKey\n  type: apiKey\n  in: header\n  parameter: X-Airmeet-Secret-Key\n  description: Community secret key, presented at POST /auth.\n  sources:\n  - openapi/airmeet-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: X-Airmeet-Access-Token\n  description: Bearer access token issued by POST /auth, valid for 30 days.\n  sources:\n  - openapi/airmeet-openapi.yml\n- name: webhookAccessKey\n  type: apiKey\n  in: header\n  parameter: x-access-key\n  description: Access key for webhook registration.\n  sources:\n  - openapi/airmeet-openapi.yml\n- name: webhookSecretKey\n  type: apiKey\n  in: header\n  parameter:\
  \ x-secret-key\n  description: Secret key for webhook registration.\n  sources:\n  - openapi/airmeet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmeet/refs/heads/main/authentication/airmeet-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Company
- Cloud Saas
- Events
- Virtual Events
- Webinars
- Event Management
- Community
- Webhooks
---
