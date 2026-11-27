---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instadash-io-openapi-generated.yml
  format: yaml
  label: Instadash API
  slug: instadash-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadash-io/openapi/_ae-authored/instadash-io-openapi-generated.yml
auth_types: []
description: Instadash uses a Bearer API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Instadash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instadash declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Instadash
provider_slug: instadash-io
scheme_count: 1
schemes:
- evidence: All CLI and MCP access uses a Bearer API key.
  header: Authorization
  how_to_obtain: Create a key via the CLI login flow (`instadash login`) which saves the key to ~/.config/instadash/config.json, or mint one directly via the API with a POST to https://instadash.io/api/keys.
  location: header
  name: Bearer API key
  type: http-bearer
slug: instadash-io-authentication
source_filename: instadash-io-authentication.yml
source_heading: Authentication Profile
source_url: https://instadash.io/docs/auth
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://instadash.io/docs/auth\nsources:\n- https://instadash.io/docs/auth\n- https://instadash.io/docs/quickstart\ndescription: Instadash uses a Bearer API key for authentication.\nschemes:\n- type: http-bearer\n  name: Bearer API key\n  evidence: All CLI and MCP access uses a Bearer API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key via the CLI login flow (`instadash login`) which saves the key to ~/.config/instadash/config.json, or mint one directly\n    via the API with a POST to https://instadash.io/api/keys.\ndocs: https://instadash.io/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/instadash-io/authentication/instadash-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Data
- Ingestion
- Mesh
- Platform
- Company
---
