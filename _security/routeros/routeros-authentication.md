---
api_key_in: []
api_specs:
- filename: routeros-bridge-api-openapi.yml
  format: yaml
  label: RouterOS Bridge API
  slug: routeros-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-bridge-api-openapi.yml
- filename: routeros-dhcp-api-openapi.yml
  format: yaml
  label: RouterOS DHCP API
  slug: routeros-dhcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-dhcp-api-openapi.yml
- filename: routeros-dns-api-openapi.yml
  format: yaml
  label: RouterOS DNS API
  slug: routeros-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-dns-api-openapi.yml
- filename: routeros-firewall-api-openapi.yml
  format: yaml
  label: RouterOS Firewall API
  slug: routeros-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-firewall-api-openapi.yml
- filename: routeros-interface-api-openapi.yml
  format: yaml
  label: RouterOS Interface API
  slug: routeros-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-interface-api-openapi.yml
- filename: routeros-ip-address-api-openapi.yml
  format: yaml
  label: RouterOS IP Address API
  slug: routeros-ip-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-ip-address-api-openapi.yml
- filename: routeros-routing-api-openapi.yml
  format: yaml
  label: RouterOS Routing API
  slug: routeros-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-routing-api-openapi.yml
- filename: routeros-system-api-openapi.yml
  format: yaml
  label: RouterOS System API
  slug: routeros-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-system-api-openapi.yml
- filename: routeros-vpn-api-openapi.yml
  format: yaml
  label: RouterOS VPN API
  slug: routeros-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-vpn-api-openapi.yml
- filename: routeros-wireless-api-openapi.yml
  format: yaml
  label: RouterOS Wireless API
  slug: routeros-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-wireless-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Routeros Authentication
name_suffix: Authentication
oauth_flows: []
overview: RouterOS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RouterOS
provider_slug: routeros
scheme_count: 1
schemes:
- description: HTTP Basic Auth using RouterOS console credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/routeros-rest-api-openapi.yml
  type: http
slug: routeros-authentication
source_filename: routeros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/routeros-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using RouterOS console credentials\n  sources:\n  - openapi/routeros-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/authentication/routeros-authentication.yml
summary_line: http · 1 scheme
tags:
- Networking
- Routers
- Network Management
- Firewall
- MikroTik
---
