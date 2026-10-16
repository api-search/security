---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bulksms-attachments-api-openapi.yml
  format: yaml
  label: BulkSMS Attachments API
  slug: bulksms-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-attachments-api-openapi.yml
- filename: bulksms-blocked-numbers-api-openapi.yml
  format: yaml
  label: BulkSMS Blocked Numbers API
  slug: bulksms-blocked-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-blocked-numbers-api-openapi.yml
- filename: bulksms-credits-api-openapi.yml
  format: yaml
  label: BulkSMS Credits API
  slug: bulksms-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-credits-api-openapi.yml
- filename: bulksms-message-api-openapi.yml
  format: yaml
  label: BulkSMS Message API
  slug: bulksms-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-message-api-openapi.yml
- filename: bulksms-profile-api-openapi.yml
  format: yaml
  label: BulkSMS Profile API
  slug: bulksms-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-profile-api-openapi.yml
- filename: bulksms-webhooks-api-openapi.yml
  format: yaml
  label: BulkSMS Webhooks API
  slug: bulksms-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bulksms Authentication
name_suffix: Authentication
oauth_flows: []
overview: BulkSMS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BulkSMS
provider_slug: bulksms
scheme_count: 1
schemes:
- description: 'The API uses HTTP Basic Auth with an **API Token** for authentication.


    API tokens can be created by logging into your account and visiting _Settings > Developer Settings > API Tokens_.


    Supply the token ID as the username and the token secret as the password. The values must be [Base64 encoded](https://en.wikipedia.org/wiki/Base64) before using them in the `Authorization` header.


    For example, if'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bulksms-openapi.yaml
  type: http
slug: bulksms-authentication
source_filename: bulksms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/bulksms-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    The API uses HTTP Basic Auth with an **API Token** for authentication.\n\n    API tokens can be created by logging into your account and visiting _Settings > Developer Settings > API Tokens_.\n\n    Supply the token ID as the username and the token secret as the password. The values must be [Base64 encoded](https://en.wikipedia.org/wiki/Base64) before using them in the `Authorization` header.\n\n    For example, if\n  sources:\n  - openapi/bulksms-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/authentication/bulksms-authentication.yml
summary_line: http · 1 scheme
tags:
- SMS
- Messaging
- Communications
- Business
- BulkSMS
---
