---
api_key_in:
- path
api_specs:
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: IP Reputation & Proxy/VPN Detection API
  slug: ip-reputation-proxy-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Email Validation API
  slug: email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Phone Number Validation API
  slug: phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Malicious URL Scanner API
  slug: malicious-url-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Device Fingerprint API
  slug: device-fingerprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Transaction Scoring API
  slug: transaction-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Leaked Data (Dark Web) API
  slug: leaked-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
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
