---
api_key_in:
- header
api_specs:
- filename: qwilt-certificate-templates-api-openapi.yml
  format: yaml
  label: Qwilt Certificate Templates API
  slug: qwilt-certificate-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-certificate-templates-api-openapi.yml
- filename: qwilt-certificates-api-openapi.yml
  format: yaml
  label: Qwilt Certificates API
  slug: qwilt-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-certificates-api-openapi.yml
- filename: qwilt-origin-allow-list-api-openapi.yml
  format: yaml
  label: Qwilt Origin Allow List API
  slug: qwilt-origin-allow-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-origin-allow-list-api-openapi.yml
- filename: qwilt-publishing-operations-api-openapi.yml
  format: yaml
  label: Qwilt Publishing Operations API
  slug: qwilt-publishing-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-publishing-operations-api-openapi.yml
- filename: qwilt-site-configurations-api-openapi.yml
  format: yaml
  label: Qwilt Site Configurations API
  slug: qwilt-site-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-site-configurations-api-openapi.yml
- filename: qwilt-sites-api-openapi.yml
  format: yaml
  label: Qwilt Sites API
  slug: qwilt-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-sites-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qwilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qwilt secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qwilt
provider_slug: qwilt
scheme_count: 2
schemes:
- description: 'API key sent as `Authorization: X-API-KEY <api-key>`.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/qwilt-certificate-manager-openapi.yml
  - openapi/qwilt-media-delivery-openapi.yml
  - openapi/qwilt-origin-allow-list-openapi.yml
  type: apiKey
- description: Bearer token from the login service (cqloudLoginToken).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qwilt-certificate-manager-openapi.yml
  - openapi/qwilt-media-delivery-openapi.yml
  - openapi/qwilt-origin-allow-list-openapi.yml
  type: http
slug: qwilt-authentication
source_filename: qwilt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qwilt-certificate-manager-openapi.yml, openapi/qwilt-media-delivery-openapi.yml,\n  openapi/qwilt-origin-allow-list-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key sent as `Authorization: X-API-KEY <api-key>`.'\n  sources:\n  - openapi/qwilt-certificate-manager-openapi.yml\n  - openapi/qwilt-media-delivery-openapi.yml\n  - openapi/qwilt-origin-allow-list-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from the login service (cqloudLoginToken).\n  sources:\n  - openapi/qwilt-certificate-manager-openapi.yml\n  - openapi/qwilt-media-delivery-openapi.yml\n  - openapi/qwilt-origin-allow-list-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/authentication/qwilt-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Media
- CDN
- Content Delivery Network
- Edge Computing
- Video Streaming
- Open Caching
- Media Delivery
- Certificates
- Infrastructure
---
