---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meshes-openapi-generated.yml
  format: yaml
  label: Meshes API
  slug: meshes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meshes/refs/heads/main/openapi/_ae-authored/meshes-openapi-generated.yml
auth_types: []
description: Meshes API uses short‑lived HS256 JWTs for machine‑to‑machine authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meshes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meshes declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Meshes
provider_slug: meshes
scheme_count: 1
schemes:
- evidence: 'Authenticated requests must include the JWT in the HTTP Authorization header using the Bearer scheme: Authorization: Bearer <jwt_token>'
  header: Authorization
  how_to_obtain: Generate a short‑lived HS256 JWT signed with your Meshes access key secret, including required claims (iss, aud, org, iat, exp) as described in the documentation.
  location: header
  name: HS256 JWT
  type: http-bearer
slug: meshes-authentication
source_filename: meshes-authentication.yml
source_heading: Authentication Profile
source_url: https://meshes.io/docs/api/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://meshes.io/docs/api/authentication\nsources:\n- https://meshes.io/docs/api/authentication\n- https://meshes.io/docs/embed/oauth-connections\n- https://meshes.io/.well-known/oauth-protected-resource\n- https://meshes.io/.well-known/oauth-authorization-server\ndescription: Meshes API uses short‑lived HS256 JWTs for machine‑to‑machine authentication.\nschemes:\n- type: http-bearer\n  name: HS256 JWT\n  evidence: 'Authenticated requests must include the JWT in the HTTP Authorization header using the Bearer scheme: Authorization: Bearer <jwt_token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a short‑lived HS256 JWT signed with your Meshes access key secret, including required claims (iss, aud, org, iat, exp)\n    as described in the documentation.\nnote: Meshes does not support OAuth 2.0; OAuth flows are absent.\ndocs: https://meshes.io/docs/api/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meshes/refs/heads/main/authentication/meshes-authentication.yml
summary_line: 1 scheme
tags:
- Company
- iPaaS
- SaaS
- Integration
- API
---
