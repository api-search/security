---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hookdeploy-openapi-generated.yml
  format: yaml
  label: HookDeploy API
  slug: hookdeploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeploy/refs/heads/main/openapi/_ae-authored/hookdeploy-openapi-generated.yml
auth_types: []
description: HookDeploy authenticates API requests using API keys passed as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hookdeploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: HookDeploy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HookDeploy
provider_slug: hookdeploy
scheme_count: 1
schemes:
- evidence: 'Every request, including GET /v1/health , requires an API key in the Authorization header: Authorization: Bearer hd_live_<your-key>'
  header: Authorization
  how_to_obtain: Create API keys in the dashboard under Settings → API Keys; the full key is shown once.
  location: header
  name: Authorization
  type: http-bearer
slug: hookdeploy-authentication
source_filename: hookdeploy-authentication.yml
source_heading: Authentication Profile
source_url: https://hookdeploy.dev/docs/organizations/api-keys/
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hookdeploy.dev/docs/organizations/api-keys/\nsources:\n- https://hookdeploy.dev/docs/organizations/api-keys/\n- https://hookdeploy.dev/docs/api/overview/\n- https://hookdeploy.dev/docs/concepts/security/\n- https://hookdeploy.dev/docs/getting-started/introduction/\ndescription: HookDeploy authenticates API requests using API keys passed as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Every request, including GET /v1/health , requires an API key in the Authorization header: Authorization: Bearer hd_live_<your-key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Create API keys in the dashboard under Settings → API Keys; the full key is shown once.\ndocs: https://hookdeploy.dev/docs/organizations/api-keys/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookdeploy/refs/heads/main/authentication/hookdeploy-authentication.yml
summary_line: 1 scheme
tags:
- Webhooks
- PrivateInfrastructure
- Security
- Integration
- DeveloperTools
---
