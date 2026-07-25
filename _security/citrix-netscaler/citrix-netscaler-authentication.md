---
api_key_in:
- cookie
- header
api_specs:
- filename: citrix-netscaler-authentication-api-openapi.yml
  format: yaml
  label: Citrix NetScaler Authentication API
  slug: citrix-netscaler-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-authentication-api-openapi.yml
- filename: citrix-netscaler-cs-virtual-server-api-openapi.yml
  format: yaml
  label: Citrix NetScaler CS Virtual Server API
  slug: citrix-netscaler-cs-virtual-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-cs-virtual-server-api-openapi.yml
- filename: citrix-netscaler-lb-virtual-server-api-openapi.yml
  format: yaml
  label: Citrix NetScaler LB Virtual Server API
  slug: citrix-netscaler-lb-virtual-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-lb-virtual-server-api-openapi.yml
- filename: citrix-netscaler-ns-config-api-openapi.yml
  format: yaml
  label: Citrix NetScaler NS Config API
  slug: citrix-netscaler-ns-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-ns-config-api-openapi.yml
- filename: citrix-netscaler-statistics-api-openapi.yml
  format: yaml
  label: Citrix NetScaler Statistics API
  slug: citrix-netscaler-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-statistics-api-openapi.yml
- filename: citrix-netscaler-system-api-openapi.yml
  format: yaml
  label: Citrix NetScaler System API
  slug: citrix-netscaler-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/openapi/citrix-netscaler-system-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Citrix Netscaler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citrix NetScaler secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
scheme_count: 2
schemes:
- description: Session-based authentication token obtained via the /config/login endpoint. Provided as a cookie with each request.
  in: cookie
  name: nitroAuthToken
  parameter: NITRO_AUTH_TOKEN
  sources:
  - openapi/citrix-netscaler-nitro-openapi.yml
  type: apiKey
- description: Per-request authentication using X-NITRO-USER and X-NITRO-PASS headers as an alternative to session-based tokens.
  in: header
  name: nitroBasicAuth
  parameter: X-NITRO-USER
  sources:
  - openapi/citrix-netscaler-nitro-openapi.yml
  type: apiKey
slug: citrix-netscaler-authentication
source_filename: citrix-netscaler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/citrix-netscaler-nitro-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: nitroAuthToken\n  type: apiKey\n  in: cookie\n  parameter: NITRO_AUTH_TOKEN\n  description: Session-based authentication token obtained via the /config/login endpoint. Provided\n    as a cookie with each request.\n  sources:\n  - openapi/citrix-netscaler-nitro-openapi.yml\n- name: nitroBasicAuth\n  type: apiKey\n  in: header\n  parameter: X-NITRO-USER\n  description: Per-request authentication using X-NITRO-USER and X-NITRO-PASS headers as an\n    alternative to session-based tokens.\n  sources:\n  - openapi/citrix-netscaler-nitro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/authentication/citrix-netscaler-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
---
