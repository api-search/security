---
api_key_in: []
api_specs:
- filename: microsoft-edge-browser-api-openapi.yml
  format: yaml
  label: Microsoft Edge Browser API
  slug: microsoft-edge-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-browser-api-openapi.yml
- filename: microsoft-edge-packages-api-openapi.yml
  format: yaml
  label: Microsoft Edge Packages API
  slug: microsoft-edge-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-packages-api-openapi.yml
- filename: microsoft-edge-pages-api-openapi.yml
  format: yaml
  label: Microsoft Edge Pages API
  slug: microsoft-edge-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-pages-api-openapi.yml
- filename: microsoft-edge-products-api-openapi.yml
  format: yaml
  label: Microsoft Edge Products API
  slug: microsoft-edge-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-products-api-openapi.yml
- filename: microsoft-edge-publishing-api-openapi.yml
  format: yaml
  label: Microsoft Edge Publishing API
  slug: microsoft-edge-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-publishing-api-openapi.yml
- filename: microsoft-edge-targets-api-openapi.yml
  format: yaml
  label: Microsoft Edge Targets API
  slug: microsoft-edge-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-targets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Edge secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Edge
provider_slug: microsoft-edge
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained from Azure Active Directory using the client credentials flow with the Microsoft Partner Center API scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-edge-addons-api.yaml
  type: http
slug: microsoft-edge-authentication
source_filename: microsoft-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-edge-addons-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained from Azure Active Directory using the client\n    credentials flow with the Microsoft Partner Center API scope.\n  sources:\n  - openapi/microsoft-edge-addons-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/authentication/microsoft-edge-authentication.yml
summary_line: http · 1 scheme
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
---
