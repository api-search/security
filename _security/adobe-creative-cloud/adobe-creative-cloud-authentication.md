---
api_key_in:
- header
api_specs:
- filename: adobe-io-events-asyncapi-original.yml
  format: yaml
  label: Adobe I/O Events
  slug: io-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/asyncapi/adobe-io-events-asyncapi-original.yml
- filename: adobe-creative-cloud-assets-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Assets API
  slug: adobe-creative-cloud-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-assets-api-openapi.yml
- filename: adobe-creative-cloud-elements-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Elements API
  slug: adobe-creative-cloud-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-elements-api-openapi.yml
- filename: adobe-creative-cloud-extraction-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Extraction API
  slug: adobe-creative-cloud-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-extraction-api-openapi.yml
- filename: adobe-creative-cloud-image-editing-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Image Editing API
  slug: adobe-creative-cloud-image-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-image-editing-api-openapi.yml
- filename: adobe-creative-cloud-image-generation-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Image Generation API
  slug: adobe-creative-cloud-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-image-generation-api-openapi.yml
- filename: adobe-creative-cloud-libraries-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Libraries API
  slug: adobe-creative-cloud-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-libraries-api-openapi.yml
- filename: adobe-creative-cloud-licensing-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Licensing API
  slug: adobe-creative-cloud-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-licensing-api-openapi.yml
- filename: adobe-creative-cloud-member-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Member API
  slug: adobe-creative-cloud-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-member-api-openapi.yml
- filename: adobe-creative-cloud-pdf-operations-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud PDF Operations API
  slug: adobe-creative-cloud-pdf-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-pdf-operations-api-openapi.yml
- filename: adobe-creative-cloud-search-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Search API
  slug: adobe-creative-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-search-api-openapi.yml
- filename: adobe-creative-cloud-utilities-api-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Utilities API
  slug: adobe-creative-cloud-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-creative-cloud-utilities-api-openapi.yml
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
- Ai Ml
- Cloud
- Creative
- Design
- Documents
- Photography
- Software-as-a-Service
- Video
---
