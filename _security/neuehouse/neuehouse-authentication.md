---
api_key_in:
- header
api_specs:
- filename: neuehouse-content-api-openapi.yml
  format: yaml
  label: NeueHouse Content API
  slug: neuehouse-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuehouse/refs/heads/main/openapi/neuehouse-content-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Neuehouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeueHouse secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NeueHouse
provider_slug: neuehouse
scheme_count: 2
schemes:
- description: WordPress Application Passwords. The live route index advertises authentication.application-passwords with an authorization endpoint at https://www.neuehouse.com/wp-admin/authorize-application.php. Credentials are issued per WordPress user from wp-admin; there is no public self-service registration.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/neuehouse-content-api-openapi.yml
  type: http
- description: Cookie authentication with an X-WP-Nonce header, used by first-party browser clients only.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/neuehouse-content-api-openapi.yml
  type: apiKey
slug: neuehouse-authentication
source_filename: neuehouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/neuehouse-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords. The live route index advertises authentication.application-passwords\n    with an authorization endpoint at https://www.neuehouse.com/wp-admin/authorize-application.php.\n    Credentials are issued per WordPress user from wp-admin; there is no public self-service\n    registration.\n  sources:\n  - openapi/neuehouse-content-api-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: Cookie authentication with an X-WP-Nonce header, used by first-party browser\n    clients only.\n  sources:\n  - openapi/neuehouse-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuehouse/refs/heads/main/authentication/neuehouse-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Hospitality
- Coworking
- Events
- Content
- WordPress
- Membership
- Real Estate
- Media
- Workspace
---
