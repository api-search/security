---
anonymous_access: false
api_key_in: []
api_specs:
- filename: controlplane-openapi-generated.yml
  format: yaml
  label: ControlPlane API
  slug: controlplane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/_ae-authored/controlplane-openapi-generated.yml
auth_types: []
description: Authentication methods for Console UI (SSO via Google, GitHub, Microsoft, SAML) and CLI (interactive login, service accounts, and token management).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Controlplane Authentication
name_suffix: Authentication
oauth_flows: []
overview: ControlPlane declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ControlPlane
provider_slug: controlplane
scheme_count: 1
schemes:
- evidence: 'Authenticate API requests using a bearer token in the Authorization header:'
  header: Authorization
  how_to_obtain: Tokens can be obtained from a service account key (generated when creating a service account) or a user access token via the CLI command `cpln profile token PROFILE_NAME`.
  location: header
  name: Bearer token
  type: http-bearer
slug: controlplane-authentication
source_filename: controlplane-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.controlplane.com/core/authentication
source_yaml: "generated: '2026-10-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.controlplane.com/core/authentication\nsources:\n- https://docs.controlplane.com/core/authentication\n- https://docs.controlplane.com/reference/workload/jwt-auth\n- https://docs.controlplane.com/cli-reference/get-started/authentication\n- https://docs.controlplane.com/quickstart/overview\ndescription: Authentication methods for Console UI (SSO via Google, GitHub, Microsoft, SAML) and CLI (interactive login, service accounts, and\n  token management).\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authenticate API requests using a bearer token in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Tokens can be obtained from a service account key (generated when creating a service account) or a user access token via the\n    CLI command `cpln profile token PROFILE_NAME`.\nnote: No OAuth2 flows, API key, or other\
  \ authentication schemes are documented for the REST API.\ndocs: https://docs.controlplane.com/core/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/authentication/controlplane-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cloud
- Virtualization
- AI
- DevOps
---
