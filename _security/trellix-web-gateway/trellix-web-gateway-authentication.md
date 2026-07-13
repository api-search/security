---
api_key_in:
- cookie
api_specs:
- filename: openapi.json
  format: json
  label: Trellix Web Gateway REST API
  slug: trellix-web-gateway-rest-api
  spec_type: OpenAPI
  url: https://docs.trellix.com/api/web-gateway/openapi.json
- filename: trellix-web-gateway-reporting-openapi.yml
  format: yaml
  label: Trellix Web Gateway Reporting API
  slug: trellix-web-gateway-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix-web-gateway/refs/heads/main/openapi/trellix-web-gateway-reporting-openapi.yml
- filename: trellix-web-gateway-policy-openapi.yml
  format: yaml
  label: Trellix Web Gateway Policy API
  slug: trellix-web-gateway-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix-web-gateway/refs/heads/main/openapi/trellix-web-gateway-policy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trellix Web Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trellix Web Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trellix Web Gateway
provider_slug: trellix-web-gateway
scheme_count: 1
schemes:
- description: Session cookie obtained via the Konfigurator REST /login endpoint.
  in: cookie
  name: cookieAuth
  parameter: JSESSIONID
  sources:
  - openapi/trellix-web-gateway-policy-openapi.yml
  - openapi/trellix-web-gateway-reporting-openapi.yml
  - openapi/trellix-web-gateway-rest-openapi.yml
  type: apiKey
slug: trellix-web-gateway-authentication
source_filename: trellix-web-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trellix-web-gateway-policy-openapi.yml, openapi/trellix-web-gateway-reporting-openapi.yml,\n  openapi/trellix-web-gateway-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: Session cookie obtained via the Konfigurator REST /login endpoint.\n  sources:\n  - openapi/trellix-web-gateway-policy-openapi.yml\n  - openapi/trellix-web-gateway-reporting-openapi.yml\n  - openapi/trellix-web-gateway-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellix-web-gateway/refs/heads/main/authentication/trellix-web-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cybersecurity
- Data Loss Prevention
- Enterprise Security
- Malware Protection
- Network Security
- SSL Inspection
- Threat Protection
- URL Filtering
- Web Gateway
---
