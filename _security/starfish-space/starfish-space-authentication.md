---
api_key_in:
- header
api_specs:
- filename: starfish-space-wordpress-openapi.yml
  format: yaml
  label: Starfish Space Website Content API
  slug: starfish-space-website-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starfish-space/refs/heads/main/openapi/starfish-space-wordpress-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Starfish Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Starfish Space secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Starfish Space
provider_slug: starfish-space
scheme_count: 2
schemes:
- description: WordPress application password (username + application password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/starfish-space-wordpress-openapi.yml
  type: http
- description: WordPress cookie authentication nonce, for same-origin requests.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/starfish-space-wordpress-openapi.yml
  type: apiKey
slug: starfish-space-authentication
source_filename: starfish-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/starfish-space-wordpress-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: WordPress application password (username + application password).\n  sources:\n  - openapi/starfish-space-wordpress-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication nonce, for same-origin requests.\n  sources:\n  - openapi/starfish-space-wordpress-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starfish-space/refs/heads/main/authentication/starfish-space-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Aerospace
- Space
- Satellites
- Satellite Servicing
- Spacecraft
- Space Robotics
- Defense
- Content Management
- Model Context Protocol
---
