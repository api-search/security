---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bluecore-authn-api-openapi.yml
  format: yaml
  label: Bluecore Authn API
  slug: bluecore-authn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-authn-api-openapi.yml
- filename: bluecore-campaignsapipublic-api-openapi.yml
  format: yaml
  label: Bluecore CampaignsAPIPublic API
  slug: bluecore-campaignsapipublic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-campaignsapipublic-api-openapi.yml
- filename: bluecore-direct-send-api-openapi.yml
  format: yaml
  label: Bluecore Direct send API
  slug: bluecore-direct-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-direct-send-api-openapi.yml
- filename: bluecore-eligibility-api-openapi.yml
  format: yaml
  label: Bluecore Eligibility API
  slug: bluecore-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-eligibility-api-openapi.yml
- filename: bluecore-profile-api-openapi.yml
  format: yaml
  label: Bluecore Profile API
  slug: bluecore-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-profile-api-openapi.yml
- filename: bluecore-transactional-api-openapi.yml
  format: yaml
  label: Bluecore Transactional API
  slug: bluecore-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-transactional-api-openapi.yml
- filename: bluecore-get-status-api-openapi.yml
  format: yaml
  label: Bluecore GET STATUS API
  slug: bluecore-get-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-get-status-api-openapi.yml
- filename: bluecore-send-email-api-openapi.yml
  format: yaml
  label: Bluecore SEND EMAIL API
  slug: bluecore-send-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-send-email-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bluecore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bluecore secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bluecore
provider_slug: bluecore
scheme_count: 1
schemes:
- description: Value for the authorization header will be Bearer followed by the token generated with the [Get access token](https://developers.bluecore.com/reference/authn_getaccesstoken#/) call.
  in: header
  name: GlooAuth
  parameter: authorization
  sources:
  - openapi/bluecore-authn-api-openapi.yml
  - openapi/bluecore-campaignsapipublic-api-openapi.yml
  - openapi/bluecore-direct-send-api-openapi.yml
  - openapi/bluecore-eligibility-api-openapi.yml
  - openapi/bluecore-profile-api-openapi.yml
  - openapi/bluecore-transactional-api-openapi.yml
  type: apiKey
slug: bluecore-authentication
source_filename: bluecore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/bluecore-authn-api-openapi.yml, openapi/bluecore-campaignsapipublic-api-openapi.yml,\n  openapi/bluecore-direct-send-api-openapi.yml, openapi/bluecore-eligibility-api-openapi.yml,\n  openapi/bluecore-profile-api-openapi.yml, openapi/bluecore-transactional-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: GlooAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: Value for the authorization header will be Bearer followed by the token generated\n    with the [Get access token](https://developers.bluecore.com/reference/authn_getaccesstoken#/)\n    call.\n  sources:\n  - openapi/bluecore-authn-api-openapi.yml\n  - openapi/bluecore-campaignsapipublic-api-openapi.yml\n  - openapi/bluecore-direct-send-api-openapi.yml\n  - openapi/bluecore-eligibility-api-openapi.yml\n  - openapi/bluecore-profile-api-openapi.yml\n  - openapi/bluecore-transactional-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/authentication/bluecore-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- E-Commerce
- Consent
---
