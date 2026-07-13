---
api_key_in:
- header
api_specs:
- filename: adobe-photoshop-api-openapi-original.yml
  format: yaml
  label: Adobe Photoshop API
  slug: photoshop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/openapi/adobe-photoshop-api-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Photoshop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Photoshop secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth Server-to-Server access token obtained from Adobe IMS at https://ims-na1.adobelogin.com/ims/token/v3 using client_credentials grant type.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-photoshop-api-openapi-original.yml
  type: http
- description: Your Adobe Developer Console Client ID.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/adobe-photoshop-api-openapi-original.yml
  type: apiKey
slug: adobe-photoshop-authentication
source_filename: adobe-photoshop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-photoshop-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth Server-to-Server access token obtained from Adobe IMS at https://ims-na1.adobelogin.com/ims/token/v3\n    using client_credentials grant type.\n  sources:\n  - openapi/adobe-photoshop-api-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your Adobe Developer Console Client ID.\n  sources:\n  - openapi/adobe-photoshop-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/authentication/adobe-photoshop-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
---
