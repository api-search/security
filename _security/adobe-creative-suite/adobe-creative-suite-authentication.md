---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Adobe Photoshop API
  slug: photoshop-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/photoshop/api/openapi.json
- filename: openapi.json
  format: json
  label: Adobe Lightroom API
  slug: lightroom-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/lightroom/api/openapi.json
- filename: openapi.json
  format: json
  label: Adobe Stock API
  slug: stock-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/stock/docs/api/openapi.json
- filename: adobe-creative-suite-firefly-openapi.yml
  format: yaml
  label: Adobe Firefly API
  slug: firefly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/openapi/adobe-creative-suite-firefly-openapi.yml
- filename: adobe-creative-suite-pdf-services-openapi.yml
  format: yaml
  label: Adobe PDF Services API
  slug: pdf-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/openapi/adobe-creative-suite-pdf-services-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Creative Suite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Creative Suite secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained from Adobe IMS
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-creative-suite-firefly-openapi.yml
  - openapi/adobe-creative-suite-pdf-services-openapi.yml
  - openapi/adobe-creative-suite-photoshop-openapi.yml
  - openapi/adobe-creative-suite-stock-openapi.yml
  type: http
- description: Adobe Stock API key (client ID) required for all operations
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/adobe-creative-suite-stock-openapi.yml
  type: apiKey
slug: adobe-creative-suite-authentication
source_filename: adobe-creative-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-creative-suite-firefly-openapi.yml, openapi/adobe-creative-suite-pdf-services-openapi.yml,\n  openapi/adobe-creative-suite-photoshop-openapi.yml, openapi/adobe-creative-suite-stock-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained from Adobe IMS\n  sources:\n  - openapi/adobe-creative-suite-firefly-openapi.yml\n  - openapi/adobe-creative-suite-pdf-services-openapi.yml\n  - openapi/adobe-creative-suite-photoshop-openapi.yml\n  - openapi/adobe-creative-suite-stock-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Adobe Stock API key (client ID) required for all operations\n  sources:\n  - openapi/adobe-creative-suite-stock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/authentication/adobe-creative-suite-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Creative
- Design
- Graphics
- Photography
- Video
---
