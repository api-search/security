---
anonymous_access: false
api_key_in: []
api_specs:
- filename: immersa-openapi-generated.yml
  format: yaml
  label: Immersa API
  slug: immersa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immersa/refs/heads/main/openapi/_ae-authored/immersa-openapi-generated.yml
auth_types: []
description: Authentication methods for Immersa MarcoPolo
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Immersa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immersa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Immersa
provider_slug: immersa
scheme_count: 1
schemes:
- evidence: Python SDK Authenticate with an API token, connect providers through hosted OAuth, run governed queries, and build agents on Marcopolo's tools.
  header: Authorization
  location: header
  name: API token
  type: http-bearer
slug: immersa-authentication
source_filename: immersa-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.marcopolo.dev/getting-started
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.marcopolo.dev/getting-started\nsources:\n- https://docs.marcopolo.dev/getting-started\n- https://docs.marcopolo.dev/getting-started/claude-plugin\n- https://docs.marcopolo.dev/getting-started/codex-plugin\n- https://docs.marcopolo.dev/getting-started/deployment-options\ndescription: Authentication methods for Immersa MarcoPolo\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: Python SDK Authenticate with an API token, connect providers through hosted OAuth, run governed queries, and build agents on Marcopolo's\n    tools.\n  location: header\n  header: Authorization\nnote: Other identity options such as Google, Microsoft, GitHub, or Email are mentioned but not described with concrete authentication details\n  on the pages.\ndocs: https://docs.marcopolo.dev/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immersa/refs/heads/main/authentication/immersa-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- DataGateway
- Platform
- Security
---
