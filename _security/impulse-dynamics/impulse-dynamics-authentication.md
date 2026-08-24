---
api_key_in:
- header
api_specs:
- filename: impulse-dynamics-wp-v2-api-openapi.yml
  format: yaml
  label: Impulse Dynamics wp/v2 API
  slug: impulse-dynamics-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impulse-dynamics/refs/heads/main/openapi/impulse-dynamics-wp-v2-api-openapi.yml
- filename: impulse-dynamics-mcp-api-openapi.yml
  format: yaml
  label: Impulse Dynamics MCP API
  slug: impulse-dynamics-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impulse-dynamics/refs/heads/main/openapi/impulse-dynamics-mcp-api-openapi.yml
- filename: impulse-dynamics-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Impulse Dynamics wp-abilities/v1 API
  slug: impulse-dynamics-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impulse-dynamics/refs/heads/main/openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml
- filename: impulse-dynamics-oembed-1-0-api-openapi.yml
  format: yaml
  label: Impulse Dynamics oEmbed/1.0 API
  slug: impulse-dynamics-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impulse-dynamics/refs/heads/main/openapi/impulse-dynamics-oembed-1-0-api-openapi.yml
- filename: impulse-dynamics-root-api-openapi.yml
  format: yaml
  label: Impulse Dynamics Root API
  slug: impulse-dynamics-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impulse-dynamics/refs/heads/main/openapi/impulse-dynamics-root-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Impulse Dynamics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impulse Dynamics secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Impulse Dynamics
provider_slug: impulse-dynamics
scheme_count: 3
schemes:
- description: 'WordPress Application Passwords. The live discovery document advertises this as the site''s only machine authentication method: authentication.application-passwords.endpoints.authorization = https://impulse-dynamics.com/wp-admin/authorize-application.php (fetched 2026-08-23).'
  name: wpApplicationPassword
  scheme: basic
  sources:
  - openapi/impulse-dynamics-mcp-api-openapi.yml
  - openapi/impulse-dynamics-oembed-1-0-api-openapi.yml
  - openapi/impulse-dynamics-root-api-openapi.yml
  - openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml
  - openapi/impulse-dynamics-wp-v2-api-openapi.yml
  type: http
- description: WordPress cookie-authentication nonce, used by same-origin browser clients.
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/impulse-dynamics-mcp-api-openapi.yml
  - openapi/impulse-dynamics-oembed-1-0-api-openapi.yml
  - openapi/impulse-dynamics-root-api-openapi.yml
  - openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml
  - openapi/impulse-dynamics-wp-v2-api-openapi.yml
  type: apiKey
- description: Bearer authentication guarding the `mcp` namespace. Anonymous POST of a JSON-RPC tools/list to https://impulse-dynamics.com/wp-json/mcp/mcp-oauth-server returned HTTP 401 `mcp_unauthorized` and to https://impulse-dynamics.com/wp-json/mcp/mcp-adapter-default-server returned HTTP 401 `rest_forbidden` on 2026-08-23. This host publishes NO RFC 8414 authorization-server metadata and NO RFC 9728 protect
  name: mcpAuth
  scheme: bearer
  sources:
  - openapi/impulse-dynamics-mcp-api-openapi.yml
  - openapi/impulse-dynamics-oembed-1-0-api-openapi.yml
  - openapi/impulse-dynamics-root-api-openapi.yml
  - openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml
  - openapi/impulse-dynamics-wp-v2-api-openapi.yml
  type: http
slug: impulse-dynamics-authentication
source_filename: impulse-dynamics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: derived\nsource: openapi/impulse-dynamics-mcp-api-openapi.yml, openapi/impulse-dynamics-oembed-1-0-api-openapi.yml,\n  openapi/impulse-dynamics-root-api-openapi.yml, openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml,\n  openapi/impulse-dynamics-wp-v2-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: wpApplicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress Application Passwords. The live discovery document advertises this\n    as the site''s only machine authentication method: authentication.application-passwords.endpoints.authorization\n    = https://impulse-dynamics.com/wp-admin/authorize-application.php (fetched 2026-08-23).'\n  sources:\n  - openapi/impulse-dynamics-mcp-api-openapi.yml\n  - openapi/impulse-dynamics-oembed-1-0-api-openapi.yml\n  - openapi/impulse-dynamics-root-api-openapi.yml\n  - openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml\n \
  \ - openapi/impulse-dynamics-wp-v2-api-openapi.yml\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie-authentication nonce, used by same-origin browser clients.\n  sources:\n  - openapi/impulse-dynamics-mcp-api-openapi.yml\n  - openapi/impulse-dynamics-oembed-1-0-api-openapi.yml\n  - openapi/impulse-dynamics-root-api-openapi.yml\n  - openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml\n  - openapi/impulse-dynamics-wp-v2-api-openapi.yml\n- name: mcpAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication guarding the `mcp` namespace. Anonymous POST of a JSON-RPC\n    tools/list to https://impulse-dynamics.com/wp-json/mcp/mcp-oauth-server returned HTTP 401\n    `mcp_unauthorized` and to https://impulse-dynamics.com/wp-json/mcp/mcp-adapter-default-server\n    returned HTTP 401 `rest_forbidden` on 2026-08-23. This host publishes NO RFC 8414 authorization-server\n    metadata and NO RFC 9728 protect\n  sources:\n \
  \ - openapi/impulse-dynamics-mcp-api-openapi.yml\n  - openapi/impulse-dynamics-oembed-1-0-api-openapi.yml\n  - openapi/impulse-dynamics-root-api-openapi.yml\n  - openapi/impulse-dynamics-wp-abilities-v1-api-openapi.yml\n  - openapi/impulse-dynamics-wp-v2-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impulse-dynamics/refs/heads/main/authentication/impulse-dynamics-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Heart Failure
- Implantable Devices
- Health Technology
- Life Sciences
- Clinical Trials
- MCP
- WordPress
---
