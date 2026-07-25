---
api_key_in:
- header
api_specs:
- filename: mastercard-developer-hub-for-fdx-apis-application-check-controller-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Application Check Controller API
  slug: mastercard-developer-hub-for-fdx-apis-application-check-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-application-check-controller-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-consent-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Consent API
  slug: mastercard-developer-hub-for-fdx-apis-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-consent-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-data-resource-apis-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Data Resource APIs API
  slug: mastercard-developer-hub-for-fdx-apis-data-resource-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-data-resource-apis-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-dynamic-client-registration-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Dynamic Client Registration API
  slug: mastercard-developer-hub-for-fdx-apis-dynamic-client-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-dynamic-client-registration-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-non-par-authorize-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Non PAR Authorize API
  slug: mastercard-developer-hub-for-fdx-apis-non-par-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-non-par-authorize-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-par-rar-authorize-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs PAR+RAR Authorize API
  slug: mastercard-developer-hub-for-fdx-apis-par-rar-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-par-rar-authorize-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-resource-token-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Resource Token API
  slug: mastercard-developer-hub-for-fdx-apis-resource-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-resource-token-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-token-introspection-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Token Introspection API
  slug: mastercard-developer-hub-for-fdx-apis-token-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-token-introspection-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-upload-data-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs Upload Data API
  slug: mastercard-developer-hub-for-fdx-apis-upload-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-upload-data-api-openapi.yml
- filename: mastercard-developer-hub-for-fdx-apis-user-apis-api-openapi.yml
  format: yaml
  label: Mastercard Developer Hub for FDX APIs User APIs API
  slug: mastercard-developer-hub-for-fdx-apis-user-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/mastercard-developer-hub-for-fdx-apis-user-apis-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mastercard Developer Hub For Fdx Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mastercard Developer Hub for FDX APIs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mastercard Developer Hub for FDX APIs
provider_slug: mastercard-fdx
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fdx-authorization-api-openapi.yaml
  type: http
- description: Authorization Token to access Secured API!
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/fdx-resource-api-openapi.yaml
  type: apiKey
slug: mastercard-developer-hub-for-fdx-apis-authentication
source_filename: mastercard-developer-hub-for-fdx-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fdx-authorization-api-openapi.yaml, openapi/fdx-resource-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/fdx-authorization-api-openapi.yaml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization Token to access Secured API!\n  sources:\n  - openapi/fdx-resource-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/authentication/mastercard-developer-hub-for-fdx-apis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Banking
- FDX
- Open Banking
---
