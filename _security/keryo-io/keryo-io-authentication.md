---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keryo-io-openapi-generated.yml
  format: yaml
  label: Keryo API
  slug: keryo-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keryo-io/openapi/_ae-authored/keryo-io-openapi-generated.yml
auth_types: []
description: Authentication methods for Keryo API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Keryo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keryo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Keryo
provider_slug: keryo-io
scheme_count: 1
schemes:
- evidence: 'Send the key in the `Authorization` header as a Bearer token:'
  header: Authorization
  how_to_obtain: Create a scoped API key via the `/api-keys` endpoints; the secret key value is returned once on creation.
  location: header
  name: API Key
  type: http-bearer
slug: keryo-io-authentication
source_filename: keryo-io-authentication.yml
source_heading: Authentication Profile
source_url: https://ovion-studio.gitbook.io/keryo-docs/developers/authentication.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ovion-studio.gitbook.io/keryo-docs/developers/authentication.md\nsources:\n- https://ovion-studio.gitbook.io/keryo-docs/developers/authentication.md\n- https://ovion-studio.gitbook.io/keryo-docs/getting-started/what-is-keryo.md\n- https://ovion-studio.gitbook.io/keryo-docs/getting-started/quickstart.md\n- https://ovion-studio.gitbook.io/keryo-docs/getting-started/creating-your-account.md\ndescription: Authentication methods for Keryo API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send the key in the `Authorization` header as a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a scoped API key via the `/api-keys` endpoints; the secret key value is returned once on creation.\nnote: OAuth 2.1 tokens are used by the MCP connector, but no OAuth flow URLs or scopes are documented on these pages.\ndocs: https://ovion-studio.gitbook.io/keryo-docs/developers/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/keryo-io/authentication/keryo-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Social Media
- Marketing
- Software-as-a-Service
- Automation
- Company
---
