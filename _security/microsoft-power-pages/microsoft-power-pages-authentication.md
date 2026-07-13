---
api_key_in:
- cookie
api_specs:
- filename: microsoft-power-pages-openapi.yml
  format: yaml
  label: Power Pages Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-pages/refs/heads/main/openapi/microsoft-power-pages-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Power Pages Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Power Pages secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Power Pages
provider_slug: microsoft-power-pages
scheme_count: 1
schemes:
- description: Power Pages uses the host portal's authenticated session for the signed-in (or anonymous) user. A CSRF token must also be supplied via the `__RequestVerificationToken` request header for non-GET requests.
  in: cookie
  name: portalSession
  parameter: .AspNet.ApplicationCookie
  sources:
  - openapi/microsoft-power-pages-openapi.yml
  type: apiKey
slug: microsoft-power-pages-authentication
source_filename: microsoft-power-pages-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-power-pages-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: portalSession\n  type: apiKey\n  in: cookie\n  parameter: .AspNet.ApplicationCookie\n  description: Power Pages uses the host portal's authenticated session for the signed-in (or\n    anonymous) user. A CSRF token must also be supplied via the `__RequestVerificationToken`\n    request header for non-GET requests.\n  sources:\n  - openapi/microsoft-power-pages-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-pages/refs/heads/main/authentication/microsoft-power-pages-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Dataverse
- Low-Code
- Microsoft
- Web Portals
---
