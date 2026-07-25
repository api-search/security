---
api_key_in: []
api_specs:
- filename: tailscale-devices-api-openapi.yml
  format: yaml
  label: Tailscale Devices API
  slug: tailscale-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-devices-api-openapi.yml
- filename: tailscale-dns-api-openapi.yml
  format: yaml
  label: Tailscale DNS API
  slug: tailscale-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-dns-api-openapi.yml
- filename: tailscale-invites-api-openapi.yml
  format: yaml
  label: Tailscale Invites API
  slug: tailscale-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-invites-api-openapi.yml
- filename: tailscale-keys-api-openapi.yml
  format: yaml
  label: Tailscale Keys API
  slug: tailscale-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-keys-api-openapi.yml
- filename: tailscale-logging-api-openapi.yml
  format: yaml
  label: Tailscale Logging API
  slug: tailscale-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-logging-api-openapi.yml
- filename: tailscale-policy-api-openapi.yml
  format: yaml
  label: Tailscale Policy API
  slug: tailscale-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-policy-api-openapi.yml
- filename: tailscale-tailnet-api-openapi.yml
  format: yaml
  label: Tailscale Tailnet API
  slug: tailscale-tailnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/openapi/tailscale-tailnet-api-openapi.yml
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
