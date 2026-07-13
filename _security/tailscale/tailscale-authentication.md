---
api_key_in: []
api_specs:
- filename: v2
  format: yaml
  label: Tailscale REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.tailscale.com/api/v2
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tailscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tailscale secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tailscale
provider_slug: tailscale
scheme_count: 2
schemes:
- description: Tailscale API access token (prefixed "tskey-api-") passed in the Authorization header. Tokens are created in the admin console with 1-90 day expiry, or via OAuth client credentials with scopes.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tailscale-openapi.yml
  type: http
- description: HTTP Basic Auth with the access token as the username and an empty password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/tailscale-openapi.yml
  type: http
slug: tailscale-authentication
source_filename: tailscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tailscale-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Tailscale API access token (prefixed \"tskey-api-\") passed in the Authorization\n    header. Tokens are created in the admin console with 1-90 day expiry, or via OAuth client\n    credentials with scopes.\n  sources:\n  - openapi/tailscale-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth with the access token as the username and an empty password.\n  sources:\n  - openapi/tailscale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/authentication/tailscale-authentication.yml
summary_line: http · 2 schemes
tags:
- VPN
- Mesh Networking
- WireGuard
- Zero Trust
- Networking
- Identity
---
