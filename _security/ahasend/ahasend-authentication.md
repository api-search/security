---
api_key_in:
- header
api_specs:
- filename: ahasend-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Accounts API
  slug: ahasend-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-accounts-api-openapi.yml
- filename: ahasend-api-keys-api-openapi.yml
  format: yaml
  label: AhaSend API Keys API
  slug: ahasend-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-api-keys-api-openapi.yml
- filename: ahasend-domains-api-openapi.yml
  format: yaml
  label: AhaSend Domains API
  slug: ahasend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-domains-api-openapi.yml
- filename: ahasend-email-api-openapi.yml
  format: yaml
  label: AhaSend Email API
  slug: ahasend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-email-api-openapi.yml
- filename: ahasend-messages-api-openapi.yml
  format: yaml
  label: AhaSend Messages API
  slug: ahasend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-messages-api-openapi.yml
- filename: ahasend-routes-api-openapi.yml
  format: yaml
  label: AhaSend Routes API
  slug: ahasend-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-routes-api-openapi.yml
- filename: ahasend-smtp-credentials-api-openapi.yml
  format: yaml
  label: AhaSend SMTP Credentials API
  slug: ahasend-smtp-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-smtp-credentials-api-openapi.yml
- filename: ahasend-statistics-api-openapi.yml
  format: yaml
  label: AhaSend Statistics API
  slug: ahasend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-statistics-api-openapi.yml
- filename: ahasend-suppressions-api-openapi.yml
  format: yaml
  label: AhaSend Suppressions API
  slug: ahasend-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-suppressions-api-openapi.yml
- filename: ahasend-utility-api-openapi.yml
  format: yaml
  label: AhaSend Utility API
  slug: ahasend-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-utility-api-openapi.yml
- filename: ahasend-webhooks-api-openapi.yml
  format: yaml
  label: AhaSend Webhooks API
  slug: ahasend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ahasend Authentication
name_suffix: Authentication
oauth_flows: []
overview: AhaSend secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AhaSend
provider_slug: ahasend
scheme_count: 2
schemes:
- bearerFormat: aha-sk-64-CHARACTER-RANDOM-STRING
  description: API key for authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ahasend-openapi-v2.yaml
  type: http
- in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/ahasend-openapi.yml
  type: apiKey
slug: ahasend-authentication
source_filename: ahasend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ahasend-openapi-v2.yaml, openapi/ahasend-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: aha-sk-64-CHARACTER-RANDOM-STRING\n  description: API key for authentication\n  sources:\n  - openapi/ahasend-openapi-v2.yaml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ahasend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/authentication/ahasend-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
---
