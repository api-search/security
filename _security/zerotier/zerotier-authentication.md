---
api_key_in:
- header
api_specs:
- filename: zerotier-central-openapi-original.json
  format: json
  label: ZeroTier Central API
  slug: zerotier-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-central-openapi-original.json
- filename: zerotier-service-openapi-original.json
  format: json
  label: ZeroTier One Service API
  slug: zerotier-one-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-service-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zerotier Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZeroTier secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ZeroTier
provider_slug: zerotier
scheme_count: 2
schemes:
- name: tokenAuth
  scheme: token
  sources:
  - openapi/zerotier-central-openapi-original.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-ZT1-Auth
  sources:
  - openapi/zerotier-service-openapi-original.json
  type: apiKey
slug: zerotier-authentication
source_filename: zerotier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zerotier-central-openapi-original.json, openapi/zerotier-service-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: token\n  sources:\n  - openapi/zerotier-central-openapi-original.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ZT1-Auth\n  sources:\n  - openapi/zerotier-service-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/authentication/zerotier-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Networking
- Software-Defined Networking
- SDN
- VPN
- Security
- Connectivity
- Overlay Network
- Zero Trust
- Infrastructure
---
