---
api_key_in:
- header
api_specs:
- filename: uveye-appraisal-api-openapi.yml
  format: yaml
  label: UVeye Appraisal API
  slug: uveye-appraisal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-appraisal-api-openapi.yml
- filename: uveye-inspections-api-openapi.yml
  format: yaml
  label: UVeye Inspections API
  slug: uveye-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-inspections-api-openapi.yml
- filename: uveye-media-api-openapi.yml
  format: yaml
  label: UVeye Media API
  slug: uveye-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-media-api-openapi.yml
- filename: uveye-merchandise-api-openapi.yml
  format: yaml
  label: UVeye Merchandise API
  slug: uveye-merchandise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-merchandise-api-openapi.yml
- filename: uveye-public-links-api-openapi.yml
  format: yaml
  label: UVeye Public Links API
  slug: uveye-public-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-public-links-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Uveye Authentication
name_suffix: Authentication
oauth_flows: []
overview: UVeye secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UVeye
provider_slug: uveye
scheme_count: 2
schemes:
- description: Global API key generated in the Global Keys tab of the UVeye Back Office.
  in: header
  name: uveyeApiKey
  parameter: uveye-api-key
  sources:
  - openapi/uveye-public-api-v1-openapi.yml
  type: apiKey
- description: 'Merchandise API key issued at onboarding, sent as `Authorization: Bearer <merchandise API key>`. Distinct from `uveye-api-key`.'
  name: merchandiseBearer
  scheme: bearer
  sources:
  - openapi/uveye-public-api-v1-openapi.yml
  type: http
slug: uveye-authentication
source_filename: uveye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://api.v1.uveye.dev/ (UVeye Public API v1 documentation v1.2) + openapi/uveye-public-api-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: uveyeApiKey\n  type: apiKey\n  in: header\n  parameter: uveye-api-key\n  description: Global API key generated in the Global Keys tab of the UVeye Back Office.\n  sources:\n  - openapi/uveye-public-api-v1-openapi.yml\n- name: merchandiseBearer\n  type: http\n  scheme: bearer\n  description: 'Merchandise API key issued at onboarding, sent as `Authorization: Bearer <merchandise\n    API key>`. Distinct from `uveye-api-key`.'\n  sources:\n  - openapi/uveye-public-api-v1-openapi.yml\ndocs: https://api.v1.uveye.dev/\nkey_management:\n  inspection_api:\n    header: uveye-api-key\n    issued_via: Global Keys tab of the UVeye Back Office\n    console: https://us.backoffice.uveye.app/\n    rotation: refresh the key in the\
  \ Back Office; a rotated-out key returns 401 \"API key is disabled\"\n  merchandise_api:\n    header: 'Authorization: Bearer <merchandise API key>'\n    issued_via: onboarding\n    note: a distinct credential from uveye-api-key; a key not authorized for merchandise returns 401\noperation_coverage:\n  uveyeApiKey:\n  - getInspectionDetails\n  - listLatestInspections\n  - createInspectionPublicLink\n  - recordInspectionShared\n  - getQuoteByInspection\n  - getInspectionImage\n  merchandiseBearer:\n  - submitMerchandiseInventory\n  - markMerchandiseVehiclesSold\nwebhook_authentication:\n  direction: UVeye -> integrator\n  bearer: 'Authorization: Bearer <customer-bearer-token> issued at onboarding; match it to authenticate\n    UVeye'\n  signature: X-UVeye-Signature, an HS256 JWT binding body_sha256 and carrying a delivery_id\n  see: asyncapi/uveye-merchandise-webhooks.yml\noauth:\n  supported: false\n  evidence: no oauth2 securityScheme; /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n\
  \    return 404 on every host\nscopes:\n  supported: false\n  note: API keys are not scoped in the published contract; see conventions for the two-credential split\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/authentication/uveye-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Automotive
- Vehicle Inspection
- Artificial Intelligence
- Computer Vision
- Dealerships
- Fleet Management
- Auctions and Remarketing
- Automotive Retail
- Inspection Data
- Company
---
