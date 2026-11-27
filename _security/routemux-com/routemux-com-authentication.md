---
anonymous_access: false
api_key_in: []
api_specs:
- filename: routemux-com-chat-completions-api-openapi.yml
  format: yaml
  label: RouteMux Chat Completions API
  slug: routemux-com-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routemux-com/openapi/routemux-com-chat-completions-api-openapi.yml
auth_types: []
description: Authentication schemes for RouteMux API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: RouteMux Authentication
name_suffix: Authentication
oauth_flows: []
overview: RouteMux declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RouteMux
provider_slug: routemux-com
scheme_count: 3
schemes:
- evidence: 'Authorization: Bearer $ROUTEMUX_API_KEY'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'x-api-key: $ROUTEMUX_API_KEY'
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'x-goog-api-key: $ROUTEMUX_API_KEY'
  header: x-goog-api-key
  location: header
  name: x-goog-api-key
  type: apiKey
slug: routemux-com-authentication
source_filename: routemux-com-authentication.yml
source_heading: Authentication Profile
source_url: https://routemux.com/docs/authentication
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://routemux.com/docs/authentication\nsources:\n- https://routemux.com/docs/authentication\n- https://routemux.com/docs/authentication\n- https://routemux.com/docs/getting-started.md\n- https://routemux.com/docs/getting-started.md\ndescription: Authentication schemes for RouteMux API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer $ROUTEMUX_API_KEY'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: x-api-key\n  evidence: 'x-api-key: $ROUTEMUX_API_KEY'\n  location: header\n  header: x-api-key\n- type: apiKey\n  name: x-goog-api-key\n  evidence: 'x-goog-api-key: $ROUTEMUX_API_KEY'\n  location: header\n  header: x-goog-api-key\nnote: Only the above header‑based schemes are documented; no OAuth2 flows are provided.\ndocs: https://routemux.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/routemux-com/authentication/routemux-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Gateways
- Multi-Model
- Unified API
- Company
---
