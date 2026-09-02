---
api_key_in:
- header
api_specs:
- filename: zerotier-controller-api-openapi.yml
  format: yaml
  label: ZeroTier controller API
  slug: zerotier-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-controller-api-openapi.yml
- filename: zerotier-network-api-openapi.yml
  format: yaml
  label: ZeroTier network API
  slug: zerotier-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-network-api-openapi.yml
- filename: zerotier-network-member-api-openapi.yml
  format: yaml
  label: ZeroTier network-member API
  slug: zerotier-network-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-network-member-api-openapi.yml
- filename: zerotier-organizations-api-openapi.yml
  format: yaml
  label: ZeroTier organizations API
  slug: zerotier-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-organizations-api-openapi.yml
- filename: zerotier-peer-api-openapi.yml
  format: yaml
  label: ZeroTier peer API
  slug: zerotier-peer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-peer-api-openapi.yml
- filename: zerotier-status-api-openapi.yml
  format: yaml
  label: ZeroTier status API
  slug: zerotier-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-status-api-openapi.yml
- filename: zerotier-user-api-openapi.yml
  format: yaml
  label: ZeroTier user API
  slug: zerotier-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-user-api-openapi.yml
- filename: zerotier-util-api-openapi.yml
  format: yaml
  label: ZeroTier util API
  slug: zerotier-util-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-util-api-openapi.yml
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
- Software Defined Networking
- SDN
- VPN
- Security
- Connectivity
- Overlay Network
- Zero Trust
- Infrastructure
---
