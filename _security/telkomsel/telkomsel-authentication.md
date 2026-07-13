---
api_key_in:
- header
api_specs:
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub SMS API
  slug: telkomsel-digihub-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub USSD API
  slug: telkomsel-digihub-ussd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Subscriber Check API
  slug: telkomsel-digihub-subscriber-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Identity Verification API
  slug: telkomsel-digihub-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Location API
  slug: telkomsel-digihub-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub SIM Swap API
  slug: telkomsel-digihub-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Consent Management API
  slug: telkomsel-digihub-consent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Scoring and Insights API
  slug: telkomsel-digihub-scoring-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Telkomsel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telkomsel secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Telkomsel
provider_slug: telkomsel
scheme_count: 3
schemes:
- description: API Key / Package Key issued per subscribed DigiHub application.
  in: header
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/telkomsel-openapi.yml
  type: apiKey
- description: SHA256(API Key + Secret Key + current epoch timestamp in seconds, UTC). Required alongside api_key on every request. See https://digihub.telkomsel.com/documentation/consumer-guide/api-authentication
  in: header
  name: SignatureAuth
  parameter: x-signature
  sources:
  - openapi/telkomsel-openapi.yml
  type: apiKey
- description: Bearer access token obtained via the OIDC CIBA flow (POST /bc-authorize then POST /token). Used by the CAMARA-style SIM Swap API.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/telkomsel-openapi.yml
  type: http
slug: telkomsel-authentication
source_filename: telkomsel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telkomsel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: API Key / Package Key issued per subscribed DigiHub application.\n  sources:\n  - openapi/telkomsel-openapi.yml\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: x-signature\n  description: SHA256(API Key + Secret Key + current epoch timestamp in seconds, UTC). Required\n    alongside api_key on every request. See https://digihub.telkomsel.com/documentation/consumer-guide/api-authentication\n  sources:\n  - openapi/telkomsel-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained via the OIDC CIBA flow (POST /bc-authorize then\n    POST /token). Used by the CAMARA-style SIM Swap API.\n  sources:\n  - openapi/telkomsel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/authentication/telkomsel-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Telecommunications
- Indonesia
- SMS
- Mobile Network
- CPaaS
- Network APIs
- Identity Verification
---
