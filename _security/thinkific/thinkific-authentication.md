---
api_key_in:
- header
api_specs:
- filename: thinkific-admin-api-openapi.yml
  format: yaml
  label: Thinkific Admin REST API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thinkific/refs/heads/main/openapi/thinkific-admin-api-openapi.yml
- filename: thinkific-webhooks-api-openapi.yml
  format: yaml
  label: Thinkific Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thinkific/refs/heads/main/openapi/thinkific-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thinkific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thinkific secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thinkific
provider_slug: thinkific
scheme_count: 3
schemes:
- name: OAuthAccessToken
  scheme: bearer
  sources:
  - openapi/thinkific-admin-api-openapi.yml
  - openapi/thinkific-webhooks-api-openapi.yml
  type: http
- description: Used together with ApiKeySubdomain
  in: header
  name: ApiKey
  parameter: X-Auth-API-Key
  sources:
  - openapi/thinkific-admin-api-openapi.yml
  type: apiKey
- description: Used together with ApiKey
  in: header
  name: ApiKeySubdomain
  parameter: X-Auth-Subdomain
  sources:
  - openapi/thinkific-admin-api-openapi.yml
  type: apiKey
slug: thinkific-authentication
source_filename: thinkific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thinkific-admin-api-openapi.yml, openapi/thinkific-webhooks-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: OAuthAccessToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/thinkific-admin-api-openapi.yml\n  - openapi/thinkific-webhooks-api-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-API-Key\n  description: Used together with ApiKeySubdomain\n  sources:\n  - openapi/thinkific-admin-api-openapi.yml\n- name: ApiKeySubdomain\n  type: apiKey\n  in: header\n  parameter: X-Auth-Subdomain\n  description: Used together with ApiKey\n  sources:\n  - openapi/thinkific-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinkific/refs/heads/main/authentication/thinkific-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Online Courses
- E-Learning
- LMS
- Course Creation
- Enrollments
- Users
- Education
- Digital Products
- Webhooks
---
