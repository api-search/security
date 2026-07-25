---
api_key_in:
- cookie
- header
api_specs:
- filename: netbox-labs-authentication-check-api-openapi.yml
  format: yaml
  label: NetBox Labs authentication-check API
  slug: netbox-labs-authentication-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-authentication-check-api-openapi.yml
- filename: netbox-labs-circuits-api-openapi.yml
  format: yaml
  label: NetBox Labs circuits API
  slug: netbox-labs-circuits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-circuits-api-openapi.yml
- filename: netbox-labs-core-api-openapi.yml
  format: yaml
  label: NetBox Labs core API
  slug: netbox-labs-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-core-api-openapi.yml
- filename: netbox-labs-dcim-api-openapi.yml
  format: yaml
  label: NetBox Labs dcim API
  slug: netbox-labs-dcim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-dcim-api-openapi.yml
- filename: netbox-labs-extras-api-openapi.yml
  format: yaml
  label: NetBox Labs extras API
  slug: netbox-labs-extras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-extras-api-openapi.yml
- filename: netbox-labs-ipam-api-openapi.yml
  format: yaml
  label: NetBox Labs ipam API
  slug: netbox-labs-ipam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-ipam-api-openapi.yml
- filename: netbox-labs-schema-api-openapi.yml
  format: yaml
  label: NetBox Labs schema API
  slug: netbox-labs-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-schema-api-openapi.yml
- filename: netbox-labs-status-api-openapi.yml
  format: yaml
  label: NetBox Labs status API
  slug: netbox-labs-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-status-api-openapi.yml
- filename: netbox-labs-tenancy-api-openapi.yml
  format: yaml
  label: NetBox Labs tenancy API
  slug: netbox-labs-tenancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-tenancy-api-openapi.yml
- filename: netbox-labs-users-api-openapi.yml
  format: yaml
  label: NetBox Labs users API
  slug: netbox-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-users-api-openapi.yml
- filename: netbox-labs-virtualization-api-openapi.yml
  format: yaml
  label: NetBox Labs virtualization API
  slug: netbox-labs-virtualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-virtualization-api-openapi.yml
- filename: netbox-labs-vpn-api-openapi.yml
  format: yaml
  label: NetBox Labs vpn API
  slug: netbox-labs-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-vpn-api-openapi.yml
- filename: netbox-labs-wireless-api-openapi.yml
  format: yaml
  label: NetBox Labs wireless API
  slug: netbox-labs-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/openapi/netbox-labs-wireless-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Netbox Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: NetBox Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NetBox Labs
provider_slug: netbox-labs
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/netbox-labs-openapi-original.json
  type: apiKey
- description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/netbox-labs-openapi-original.json
  type: apiKey
slug: netbox-labs-authentication
source_filename: netbox-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/netbox-labs-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/netbox-labs-openapi-original.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Token <token>` (v1) or `Bearer <key>.<token>` (v2)'\n  sources:\n  - openapi/netbox-labs-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbox-labs/refs/heads/main/authentication/netbox-labs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Networking
- DCIM
- IPAM
- Infrastructure
- Source of Truth
- Network Automation
- OpenAPI
- MCP
---
