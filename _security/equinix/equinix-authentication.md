---
api_key_in:
- header
api_specs:
- filename: fabric-openapi-original.yml
  format: yaml
  label: Equinix Fabric API
  slug: fabric
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/fabric-openapi-original.yml
- filename: metal-openapi-original.yml
  format: yaml
  label: Equinix Metal API
  slug: metal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/metal-openapi-original.yml
- filename: eia-openapi-original.yml
  format: yaml
  label: Equinix Internet Access API
  slug: internet-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/eia-openapi-original.yml
- filename: lookup-openapi-original.yml
  format: yaml
  label: Equinix Lookup API
  slug: lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/lookup-openapi-original.yml
- filename: orders-openapi-original.yml
  format: yaml
  label: Equinix Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/orders-openapi-original.yml
- filename: orderhistory-openapi-original.yml
  format: yaml
  label: Equinix Order History API
  slug: order-history
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/orderhistory-openapi-original.yml
- filename: securecabinet-openapi-original.yml
  format: yaml
  label: Equinix Secure Cabinet API
  slug: secure-cabinet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/securecabinet-openapi-original.yml
- filename: smarthands-openapi-original.yml
  format: yaml
  label: Equinix Smart Hands API
  slug: smart-hands
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/smarthands-openapi-original.yml
- filename: accesstoken-openapi-original.yml
  format: yaml
  label: Equinix API Authentication
  slug: access-token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/accesstoken-openapi-original.yml
- filename: sts-openapi-original.yml
  format: yaml
  label: Equinix Security Token Service
  slug: sts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/openapi/sts-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Equinix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Equinix secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Equinix
provider_slug: equinix
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/eia-openapi-original.yml
  - openapi/lookup-openapi-original.yml
  - openapi/orders-openapi-original.yml
  - openapi/securecabinet-openapi-original.yml
  - openapi/sts-openapi-original.yml
  type: http
- description: HTTP header containing the User or Project API key that will be used to authenticate the request.
  in: header
  name: x_auth_token
  parameter: X-Auth-Token
  sources:
  - openapi/metal-openapi-original.yml
  type: apiKey
slug: equinix-authentication
source_filename: equinix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eia-openapi-original.yml, openapi/lookup-openapi-original.yml, openapi/metal-openapi-original.yml,\n  openapi/orders-openapi-original.yml, openapi/securecabinet-openapi-original.yml, openapi/sts-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/eia-openapi-original.yml\n  - openapi/lookup-openapi-original.yml\n  - openapi/orders-openapi-original.yml\n  - openapi/securecabinet-openapi-original.yml\n  - openapi/sts-openapi-original.yml\n- name: x_auth_token\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: HTTP header containing the User or Project API key that will be used to authenticate\n    the request.\n  sources:\n  - openapi/metal-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equinix/refs/heads/main/authentication/equinix-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Fortune 1000
- Data Centers
- Interconnection
- Colocation
- Bare Metal
- Cloud Infrastructure
- Networking
---
