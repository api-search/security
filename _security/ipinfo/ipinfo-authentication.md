---
api_key_in:
- query
api_specs:
- filename: ipinfo-openapi.yml
  format: yaml
  label: IPinfo Core API
  slug: ipinfo-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/main/openapi/ipinfo-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ipinfo Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPinfo secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IPinfo
provider_slug: ipinfo
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/ipinfo-openapi.yml
  type: http
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ipinfo-openapi.yml
  type: http
- in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/ipinfo-openapi.yml
  type: apiKey
slug: ipinfo-authentication
source_filename: ipinfo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ipinfo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/ipinfo-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ipinfo-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/ipinfo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/authentication/ipinfo-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- IP Intelligence
- IP Geolocation
- ASN
- Privacy Detection
- VPN Detection
- Threat Intelligence
- Network Data
- Mobile Carrier
- WHOIS
- Public APIs
- Development
---
