---
api_key_in:
- path
api_specs:
- filename: ipqualityscore-device-fingerprint-api-openapi.yml
  format: yaml
  label: IPQualityScore Device Fingerprint API
  slug: ipqualityscore-device-fingerprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-device-fingerprint-api-openapi.yml
- filename: ipqualityscore-email-validation-api-openapi.yml
  format: yaml
  label: IPQualityScore Email Validation API
  slug: ipqualityscore-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-email-validation-api-openapi.yml
- filename: ipqualityscore-ip-reputation-api-openapi.yml
  format: yaml
  label: IPQualityScore IP Reputation API
  slug: ipqualityscore-ip-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-ip-reputation-api-openapi.yml
- filename: ipqualityscore-leaked-data-api-openapi.yml
  format: yaml
  label: IPQualityScore Leaked Data API
  slug: ipqualityscore-leaked-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-leaked-data-api-openapi.yml
- filename: ipqualityscore-phone-validation-api-openapi.yml
  format: yaml
  label: IPQualityScore Phone Validation API
  slug: ipqualityscore-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-phone-validation-api-openapi.yml
- filename: ipqualityscore-url-scanner-api-openapi.yml
  format: yaml
  label: IPQualityScore URL Scanner API
  slug: ipqualityscore-url-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-url-scanner-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ipqualityscore Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPQualityScore secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IPQualityScore
provider_slug: ipqualityscore
scheme_count: 1
schemes:
- description: IPQualityScore API key passed as a path parameter on each request.
  in: path
  name: ApiKeyPath
  parameter: api_key
  sources:
  - openapi/ipqualityscore-openapi.yml
  type: apiKey
slug: ipqualityscore-authentication
source_filename: ipqualityscore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ipqualityscore-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\nschemes:\n- name: ApiKeyPath\n  type: apiKey\n  in: path\n  parameter: api_key\n  description: IPQualityScore API key passed as a path parameter on each request.\n  sources:\n  - openapi/ipqualityscore-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/authentication/ipqualityscore-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fraud Prevention
- IP Reputation
- Proxy Detection
- Email Validation
- Threat Intelligence
---
