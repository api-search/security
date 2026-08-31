---
api_key_in: []
api_specs:
- filename: mavenir-onetoonecall-api-openapi.yml
  format: yaml
  label: Mavenir One To One Call API
  slug: mavenir-onetoonecall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/openapi/mavenir-onetoonecall-api-openapi.yml
- filename: mavenir-push-token-api-openapi.yml
  format: yaml
  label: Mavenir Push Token API
  slug: mavenir-push-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/openapi/mavenir-push-token-api-openapi.yml
- filename: mavenir-racm-api-openapi.yml
  format: yaml
  label: Mavenir RACM API
  slug: mavenir-racm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/openapi/mavenir-racm-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mavenir Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mavenir secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mavenir
provider_slug: mavenir
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mavenir-byon-call-handling-openapi.yml
  - openapi/mavenir-byon-racm-openapi.yml
  type: http
slug: mavenir-authentication
source_filename: mavenir-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/mavenir-byon-call-handling-openapi.yml, openapi/mavenir-byon-racm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mavenir-byon-call-handling-openapi.yml\n  - openapi/mavenir-byon-racm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/authentication/mavenir-authentication.yml
summary_line: http · 1 scheme
tags:
- Telecommunications
- United States
- Network Vendor
- Network APIs
- CAMARA
- Open Gateway
- BSS
- OSS
- TM Forum
- Open RAN
- 5G
- IMS
- Messaging
- Network Exposure Function
- Standards
---
