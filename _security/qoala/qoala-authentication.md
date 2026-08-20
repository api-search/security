---
api_key_in:
- header
api_specs:
- filename: qoala-authentication-api-openapi.yml
  format: yaml
  label: Qoala Authentication API
  slug: qoala-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qoala/refs/heads/main/openapi/qoala-authentication-api-openapi.yml
- filename: qoala-api-specification-api-openapi.yml
  format: yaml
  label: Qoala API Specification API
  slug: qoala-api-specification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qoala/refs/heads/main/openapi/qoala-api-specification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Qoala Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qoala secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qoala
provider_slug: qoala
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/qoala-bus-insurance-openapi.yml
  - openapi/qoala-claim-api-alt-openapi.yml
  - openapi/qoala-claim-api-openapi.yml
  - openapi/qoala-credit-insurance-openapi.yml
  - openapi/qoala-credit-life-insurance-openapi.yml
  - openapi/qoala-experience-event-insurance-openapi.yml
  - openapi/qoala-flight-insurance-openapi.yml
  - openapi/qoala-gadget-insurance-openapi.yml
  - openapi/qoala-goods-insurance-openapi.yml
  - openapi/qoala-hotel-insurance-openapi.yml
  - openapi/qoala-logistic-insurance-openapi.yml
  - openapi/qoala-micro-health-insurance-openapi.yml
  - openapi/qoala-train-insurance-openapi.yml
  - openapi/qoala-vehicle-insurance-openapi.yml
  type: apiKey
slug: qoala-authentication
source_filename: qoala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/qoala-bus-insurance-openapi.yml, openapi/qoala-claim-api-alt-openapi.yml, openapi/qoala-claim-api-openapi.yml,\n  openapi/qoala-credit-insurance-openapi.yml, openapi/qoala-credit-life-insurance-openapi.yml, openapi/qoala-experience-event-insurance-openapi.yml,\n  openapi/qoala-flight-insurance-openapi.yml, openapi/qoala-gadget-insurance-openapi.yml, openapi/qoala-goods-insurance-openapi.yml,\n  openapi/qoala-hotel-insurance-openapi.yml, openapi/qoala-logistic-insurance-openapi.yml, openapi/qoala-micro-health-insurance-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/qoala-bus-insurance-openapi.yml\n  - openapi/qoala-claim-api-alt-openapi.yml\n  - openapi/qoala-claim-api-openapi.yml\n  - openapi/qoala-credit-insurance-openapi.yml\n  - openapi/qoala-credit-life-insurance-openapi.yml\n\
  \  - openapi/qoala-experience-event-insurance-openapi.yml\n  - openapi/qoala-flight-insurance-openapi.yml\n  - openapi/qoala-gadget-insurance-openapi.yml\n  - openapi/qoala-goods-insurance-openapi.yml\n  - openapi/qoala-hotel-insurance-openapi.yml\n  - openapi/qoala-logistic-insurance-openapi.yml\n  - openapi/qoala-micro-health-insurance-openapi.yml\n  - openapi/qoala-train-insurance-openapi.yml\n  - openapi/qoala-vehicle-insurance-openapi.yml\ndocs: https://docs.qoala.app/reference/authentication\nissuance: Partner API keys are issued by Qoala Engineering during integration onboarding; there is no self-service key\n  request.\nheader_example: 'x-api-key: <partner-api-key>'\nplatform_session_api:\n  note: Separate from partner API-key auth. The Authentication API (openapi/qoala-authentication-api-openapi.yml) issues\n    a JWT access token and refresh token for the Qoala for Enterprise platform via passwordless email + security code.\n  operations:\n  - createSession (POST /v2/sessions)\n\
  \  - refreshSession (POST /v2/sessions/refresh)\n  required_headers:\n  - priority\n  - x-captcha-token (createSession only)\n  note_security: This spec is the only Qoala specification that does not declare the ApiKeyAuth scheme.\noauth2: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qoala/refs/heads/main/authentication/qoala-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Policies
- Claims
- Southeast Asia
- Indonesia
- Financial-Services
- Partner API
---
