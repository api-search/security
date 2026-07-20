---
api_key_in: []
api_specs:
- filename: kolide-k2-openapi.json
  format: json
  label: Kolide K2 API
  slug: kolide-k2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-k2-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kolide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kolide secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kolide
provider_slug: kolide
scheme_count: 1
schemes:
- applied: 'globally via root-level security [{api_key: []}] on all 65 operations'
  authorization:
    model: per-key permissions
    read: available to all plans
    scopes: none — Kolide does not expose an OAuth scope surface
    write: Available exclusively to Kolide Max subscribers. Write access must be granted explicitly per key and requires a documented rationale at creation time.
  format: 'Authorization: Bearer $KOLIDE_API_TOKEN'
  header: Authorization
  in: header
  name: api_key
  provisioning:
    required_role: administrator
    ui_path: Settings > Developers > API Keys
  scheme: bearer
  sources:
  - openapi/kolide-k2-openapi.json
  - openapi/kolide-k2-2023-05-26-openapi.json
  token:
    example_documented_by_provider: k2sk_v1_A2UYhW7OPt2jKKLqmFcaGNK7
    expiry: not documented
    prefix: k2sk
    rotation: manual, via the admin dashboard
    shape: $PREFIX_$VERSION_$SECRET
    version_segment: v1
  type: http
slug: kolide-authentication
source_filename: kolide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource:\n- https://www.kolide.com/docs/developers/api\n- openapi/kolide-k2-openapi.json\n- openapi/kolide-k2-2023-05-26-openapi.json\ndocs: https://www.kolide.com/docs/developers/api\napi: K2 API\nbase_url: https://api.kolide.com\nsummary:\n  types: [http]\n  model: static bearer API keys — no OAuth authorization server, no scopes, no OIDC\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer $KOLIDE_API_TOKEN'\n  applied: 'globally via root-level security [{api_key: []}] on all 65 operations'\n  sources:\n  - openapi/kolide-k2-openapi.json\n  - openapi/kolide-k2-2023-05-26-openapi.json\n  token:\n    shape: $PREFIX_$VERSION_$SECRET\n    prefix: k2sk\n    version_segment: v1\n    example_documented_by_provider: k2sk_v1_A2UYhW7OPt2jKKLqmFcaGNK7\n    rotation: manual, via the admin dashboard\n    expiry: not documented\n  provisioning:\n    ui_path: Settings\
  \ > Developers > API Keys\n    required_role: administrator\n  authorization:\n    model: per-key permissions\n    read: available to all plans\n    write: >-\n      Available exclusively to Kolide Max subscribers. Write access must be granted\n      explicitly per key and requires a documented rationale at creation time.\n    scopes: none — Kolide does not expose an OAuth scope surface\nsecondary_credentials:\n- name: SSF poll bearer token\n  header: X-Kolide-Poll-Bearer-Token\n  applies_to: SSF stream polling (RFC 8936)\n  rotation: 'POST /ssf_streams/{id}/rotate_poll_token with overlap | immediate | disable modes'\n  source: https://www.kolide.com/docs/developers/ssf-streams\n- name: webhook signing secret\n  header: Authorization\n  algorithm: HMAC-SHA256 hex digest over the raw request body\n  applies_to: inbound webhook verification\n  source: https://www.kolide.com/docs/developers/webhooks\nrelated_headers:\n- name: X-Kolide-Api-Version\n  purpose: Pin the dated API version line\
  \ (current 2026-04-07); optional, defaults to latest\ngaps:\n- No OAuth 2.0 or OpenID Connect support; no /.well-known/oauth-authorization-server or\n  /.well-known/openid-configuration (both 404).\n- No scope surface — permissions are coarse per-key grants, not delegatable scopes.\n- No documented token expiry or automated rotation for the primary k2sk API key.\n- No mutual TLS or request-signing option for API calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/authentication/kolide-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- B2B
- Security
- Device Trust
- Endpoint Security
- Zero Trust
- Compliance
- Identity
- osquery
- Device Management
---
