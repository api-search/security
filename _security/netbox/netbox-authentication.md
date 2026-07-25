---
api_key_in:
- cookie
- header
api_specs:
- filename: netbox-authentication-check-api-openapi.yml
  format: yaml
  label: NetBox authentication-check API
  slug: netbox-authentication-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-authentication-check-api-openapi.yml
- filename: netbox-circuits-api-openapi.yml
  format: yaml
  label: NetBox circuits API
  slug: netbox-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-circuits-api-openapi.yml
- filename: netbox-core-api-openapi.yml
  format: yaml
  label: NetBox core API
  slug: netbox-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-core-api-openapi.yml
- filename: netbox-dcim-api-openapi.yml
  format: yaml
  label: NetBox dcim API
  slug: netbox-dcim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-dcim-api-openapi.yml
- filename: netbox-extras-api-openapi.yml
  format: yaml
  label: NetBox extras API
  slug: netbox-extras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-extras-api-openapi.yml
- filename: netbox-ipam-api-openapi.yml
  format: yaml
  label: NetBox ipam API
  slug: netbox-ipam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-ipam-api-openapi.yml
- filename: netbox-schema-api-openapi.yml
  format: yaml
  label: NetBox schema API
  slug: netbox-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-schema-api-openapi.yml
- filename: netbox-status-api-openapi.yml
  format: yaml
  label: NetBox status API
  slug: netbox-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-status-api-openapi.yml
- filename: netbox-tenancy-api-openapi.yml
  format: yaml
  label: NetBox tenancy API
  slug: netbox-tenancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-tenancy-api-openapi.yml
- filename: netbox-users-api-openapi.yml
  format: yaml
  label: NetBox users API
  slug: netbox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-users-api-openapi.yml
- filename: netbox-virtualization-api-openapi.yml
  format: yaml
  label: NetBox virtualization API
  slug: netbox-virtualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-virtualization-api-openapi.yml
- filename: netbox-vpn-api-openapi.yml
  format: yaml
  label: NetBox vpn API
  slug: netbox-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-vpn-api-openapi.yml
- filename: netbox-wireless-api-openapi.yml
  format: yaml
  label: NetBox wireless API
  slug: netbox-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/openapi/netbox-wireless-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Netbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetBox secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetBox
provider_slug: netbox
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/netbox-openapi.yml
  type: apiKey
- description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/netbox-openapi.yml
  type: apiKey
slug: netbox-authentication
source_filename: netbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netbox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/netbox-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'\n  sources:\n  - openapi/netbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbox/refs/heads/main/authentication/netbox-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data Center
- DCIM
- Infrastructure as Code
- IPAM
- Network Automation
- Network Management
- Open Source
- Source of Truth
---
