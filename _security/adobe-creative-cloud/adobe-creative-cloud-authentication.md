---
api_key_in:
- header
api_specs:
- filename: adobe-firefly-api-openapi-original.yml
  format: yaml
  label: Adobe Firefly API
  slug: firefly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-firefly-api-openapi-original.yml
- filename: adobe-cc-libraries-api-openapi-original.yml
  format: yaml
  label: Creative Cloud Libraries API
  slug: cc-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-cc-libraries-api-openapi-original.yml
- filename: adobe-stock-api-openapi-original.yml
  format: yaml
  label: Adobe Stock API
  slug: stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-stock-api-openapi-original.yml
- filename: adobe-pdf-services-api-openapi-original.yml
  format: yaml
  label: Adobe PDF Services API
  slug: pdf-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-pdf-services-api-openapi-original.yml
- filename: adobe-io-events-asyncapi-original.yml
  format: yaml
  label: Adobe I/O Events
  slug: io-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/asyncapi/adobe-io-events-asyncapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Creative Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Creative Cloud secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-cc-libraries-api-openapi-original.yml
  - openapi/adobe-firefly-api-openapi-original.yml
  - openapi/adobe-pdf-services-api-openapi-original.yml
  - openapi/adobe-stock-api-openapi-original.yml
  type: http
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/adobe-cc-libraries-api-openapi-original.yml
  - openapi/adobe-firefly-api-openapi-original.yml
  - openapi/adobe-pdf-services-api-openapi-original.yml
  - openapi/adobe-stock-api-openapi-original.yml
  type: apiKey
slug: adobe-creative-cloud-authentication
source_filename: adobe-creative-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-cc-libraries-api-openapi-original.yml, openapi/adobe-firefly-api-openapi-original.yml,\n  openapi/adobe-pdf-services-api-openapi-original.yml, openapi/adobe-stock-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/adobe-cc-libraries-api-openapi-original.yml\n  - openapi/adobe-firefly-api-openapi-original.yml\n  - openapi/adobe-pdf-services-api-openapi-original.yml\n  - openapi/adobe-stock-api-openapi-original.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/adobe-cc-libraries-api-openapi-original.yml\n  - openapi/adobe-firefly-api-openapi-original.yml\n  - openapi/adobe-pdf-services-api-openapi-original.yml\n  - openapi/adobe-stock-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/authentication/adobe-creative-cloud-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
---
