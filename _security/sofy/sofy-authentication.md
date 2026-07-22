---
api_key_in:
- header
api_specs:
- filename: sofy-public-api-openapi.yml
  format: yaml
  label: SOFY Public API
  slug: sofy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofy/refs/heads/main/openapi/sofy-public-api-openapi.yml
auth_types:
- apiKey
description: SOFY's public API authenticates with a single API access key passed in the `x-sofy-auth-key` request header. The key is generated in the SOFY web app under Account Settings > API Key and is scoped to the subscription. There is no OAuth or OpenID Connect surface; the key is a bearer-style secret with no per-scope granularity.
kind: authentication
layout: security
method: searched
name: Sofy Authentication
name_suffix: Authentication
oauth_flows: []
overview: SOFY secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SOFY
provider_slug: sofy
scheme_count: 1
schemes:
- description: Subscription API key from Account > Account Settings > API Key. Required on every request. A missing header returns 400 "Missing required headers"; an invalid/expired key returns 401 "No user found".
  in: header
  key_name: x-sofy-auth-key
  name: sofyAuthKey
  sources:
  - openapi/sofy-public-api-openapi.yml
  type: apiKey
slug: sofy-authentication
source_filename: sofy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sofy.ai/account-setting/generating-api-access-keys\ndocs: https://docs.sofy.ai/account-setting/generating-api-access-keys\ndescription: >-\n  SOFY's public API authenticates with a single API access key passed in the\n  `x-sofy-auth-key` request header. The key is generated in the SOFY web app\n  under Account Settings > API Key and is scoped to the subscription. There is\n  no OAuth or OpenID Connect surface; the key is a bearer-style secret with no\n  per-scope granularity.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\nschemes:\n  - name: sofyAuthKey\n    type: apiKey\n    in: header\n    key_name: x-sofy-auth-key\n    description: >-\n      Subscription API key from Account > Account Settings > API Key. Required on\n      every request. A missing header returns 400 \"Missing required headers\"; an\n      invalid/expired key returns 401 \"No user found\".\n    sources:\n\
  \      - openapi/sofy-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofy/refs/heads/main/authentication/sofy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Testing
- Test Automation
- Mobile Testing
- QA
- No-Code
- Continuous Testing
- DevOps
---
