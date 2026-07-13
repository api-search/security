---
api_key_in:
- header
api_specs:
- filename: mubert-music-api-openapi.yml
  format: yaml
  label: Mubert AI Music API
  slug: mubert-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mubert/refs/heads/main/openapi/mubert-music-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mubert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mubert secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mubert
provider_slug: mubert
scheme_count: 4
schemes:
- description: Mubert customer identifier (public endpoints).
  in: header
  name: customerId
  parameter: customer-id
  sources:
  - openapi/mubert-music-api-openapi.yml
  type: apiKey
- description: Mubert customer access token (public endpoints).
  in: header
  name: accessToken
  parameter: access-token
  sources:
  - openapi/mubert-music-api-openapi.yml
  type: apiKey
- description: Mubert company identifier (service endpoints).
  in: header
  name: companyId
  parameter: company-id
  sources:
  - openapi/mubert-music-api-openapi.yml
  type: apiKey
- description: Mubert license token (service endpoints).
  in: header
  name: licenseToken
  parameter: license-token
  sources:
  - openapi/mubert-music-api-openapi.yml
  type: apiKey
slug: mubert-authentication
source_filename: mubert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mubert-music-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: customerId\n  type: apiKey\n  in: header\n  parameter: customer-id\n  description: Mubert customer identifier (public endpoints).\n  sources:\n  - openapi/mubert-music-api-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: access-token\n  description: Mubert customer access token (public endpoints).\n  sources:\n  - openapi/mubert-music-api-openapi.yml\n- name: companyId\n  type: apiKey\n  in: header\n  parameter: company-id\n  description: Mubert company identifier (service endpoints).\n  sources:\n  - openapi/mubert-music-api-openapi.yml\n- name: licenseToken\n  type: apiKey\n  in: header\n  parameter: license-token\n  description: Mubert license token (service endpoints).\n  sources:\n  - openapi/mubert-music-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mubert/refs/heads/main/authentication/mubert-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- AI Music
- Generative
- Royalty-Free
- Streaming
- Text-to-Music
- Image-to-Music
- Stems
- B2B
---
