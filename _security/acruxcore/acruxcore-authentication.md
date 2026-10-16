---
anonymous_access: false
api_key_in: []
api_specs:
- filename: acruxcore-openapi-generated.yml
  format: yaml
  label: Acrux Core API
  slug: acruxcore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/_ae-authored/acruxcore-openapi-generated.yml
auth_types: []
description: Every endpoint authenticates with a Bearer API key in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Acruxcore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acrux Core declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Acrux Core
provider_slug: acruxcore
scheme_count: 1
schemes:
- evidence: 'Every endpoint in this reference authenticates the same way: a Bearer API key in the Authorization header.'
  header: Authorization
  how_to_obtain: Generate a key in the dashboard (Account & keys → New key) and export it as an environment variable.
  location: header
  name: API Key
  type: http-bearer
slug: acruxcore-authentication
source_filename: acruxcore-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.acruxcore.com/api-reference/api-keys
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.acruxcore.com/api-reference/api-keys\nsources:\n- https://docs.acruxcore.com/api-reference/api-keys\n- https://docs.acruxcore.com/api-reference/authentication\n- https://docs.acruxcore.com/docs/getting-started/quickstart\n- https://docs.acruxcore.com/docs/getting-started/core-concepts\ndescription: Every endpoint authenticates with a Bearer API key in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every endpoint in this reference authenticates the same way: a Bearer API key in the Authorization header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key in the dashboard (Account & keys → New key) and export it as an environment variable.\ndocs: https://docs.acruxcore.com/api-reference/api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/authentication/acruxcore-authentication.yml
summary_line: 1 scheme
tags:
- LLMOps
- OpenSource
- Platform
- Engineering
- AI
---
