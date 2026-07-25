---
api_key_in: []
api_specs:
- filename: smsapi-2fa-api-openapi.yml
  format: yaml
  label: SMSAPI 2FA API
  slug: smsapi-2fa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-2fa-api-openapi.yml
- filename: smsapi-blacklist-api-openapi.yml
  format: yaml
  label: SMSAPI Blacklist API
  slug: smsapi-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-blacklist-api-openapi.yml
- filename: smsapi-contacts-api-openapi.yml
  format: yaml
  label: SMSAPI Contacts API
  slug: smsapi-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-contacts-api-openapi.yml
- filename: smsapi-hlr-api-openapi.yml
  format: yaml
  label: SMSAPI HLR API
  slug: smsapi-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-hlr-api-openapi.yml
- filename: smsapi-mms-api-openapi.yml
  format: yaml
  label: SMSAPI MMS API
  slug: smsapi-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-mms-api-openapi.yml
- filename: smsapi-profile-api-openapi.yml
  format: yaml
  label: SMSAPI Profile API
  slug: smsapi-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-profile-api-openapi.yml
- filename: smsapi-sender-names-api-openapi.yml
  format: yaml
  label: SMSAPI Sender Names API
  slug: smsapi-sender-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-sender-names-api-openapi.yml
- filename: smsapi-short-urls-api-openapi.yml
  format: yaml
  label: SMSAPI Short URLs API
  slug: smsapi-short-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-short-urls-api-openapi.yml
- filename: smsapi-sms-api-openapi.yml
  format: yaml
  label: SMSAPI SMS API
  slug: smsapi-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-sms-api-openapi.yml
- filename: smsapi-subusers-api-openapi.yml
  format: yaml
  label: SMSAPI Subusers API
  slug: smsapi-subusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-subusers-api-openapi.yml
- filename: smsapi-vms-api-openapi.yml
  format: yaml
  label: SMSAPI VMS API
  slug: smsapi-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-vms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SMSAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SMSAPI
provider_slug: smsapi
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token generated in the SMSAPI customer panel (API Tokens).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smsapi-openapi.yml
  type: http
slug: smsapi-authentication
source_filename: smsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smsapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token generated in the SMSAPI customer panel (API Tokens).\n  sources:\n  - openapi/smsapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/authentication/smsapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Messaging
- SMS
- MMS
- Voice
- 2FA
- Bulk Messaging
- Communications
- CPaaS
---
