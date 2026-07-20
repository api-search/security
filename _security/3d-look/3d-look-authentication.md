---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 3D Look Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3D Look secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 3D Look
provider_slug: 3d-look
scheme_count: 2
schemes:
- api: SAIA Perfect Fit / Mobile Tailor (MTM) API
  docs: https://saia.3dlook.me/docs/
  format: APIKey <YOUR_API_KEY>
  in: header
  key_source: Mobile Tailor admin panel
  name: SaiaApiKey
  parameter: Authorization
  sources:
  - https://saia.3dlook.me/docs/
  type: apiKey
- api: FitXpress API
  docs: https://docs.fitxpress.3dlook.me/
  format: Token <ACCESS_TOKEN>
  in: header
  name: FitXpressToken
  parameter: Authorization
  sources:
  - https://docs.fitxpress.3dlook.me/
  type: apiKey
slug: 3d-look-authentication
source_filename: 3d-look-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://saia.3dlook.me/docs/ ; https://docs.fitxpress.3dlook.me/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: API-key / token authentication carried in the Authorization header; no OAuth2 surface documented.\nschemes:\n- name: SaiaApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: \"APIKey <YOUR_API_KEY>\"\n  api: SAIA Perfect Fit / Mobile Tailor (MTM) API\n  docs: https://saia.3dlook.me/docs/\n  key_source: Mobile Tailor admin panel\n  sources: [https://saia.3dlook.me/docs/]\n- name: FitXpressToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: \"Token <ACCESS_TOKEN>\"\n  api: FitXpress API\n  docs: https://docs.fitxpress.3dlook.me/\n  sources: [https://docs.fitxpress.3dlook.me/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3d-look/refs/heads/main/authentication/3d-look-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Body Measurement
- Computer Vision
- Artificial Intelligence
- Apparel
- Fashion Technology
- Health and Fitness
- Sizing
- 3D Body Scanning
- SDK
---
