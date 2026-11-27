---
anonymous_access: false
api_key_in: []
api_specs:
- filename: triplebooks-com-openapi-generated.yml
  format: yaml
  label: TripleBooks API
  slug: triplebooks-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/triplebooks-com/openapi/_ae-authored/triplebooks-com-openapi-generated.yml
auth_types: []
description: Authentication uses a Bearer token containing an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: TripleBooks Authentication
name_suffix: Authentication
oauth_flows: []
overview: TripleBooks declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TripleBooks
provider_slug: triplebooks-com
scheme_count: 1
schemes:
- evidence: 'Authentication: Authorization: Bearer ak_... using an API key from API keys in Settings.'
  header: Authorization
  how_to_obtain: Create keys under Settings → API keys.
  location: header
  name: Bearer
  type: http-bearer
slug: triplebooks-com-authentication
source_filename: triplebooks-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.triplebooks.com/api/platform/api-keys
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.triplebooks.com/api/platform/api-keys\nsources:\n- https://docs.triplebooks.com/api/platform/api-keys\n- https://docs.triplebooks.com/api\ndescription: Authentication uses a Bearer token containing an API key.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authentication: Authorization: Bearer ak_... using an API key from API keys in Settings.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys under Settings → API keys.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://docs.triplebooks.com/api/platform/api-keys\n"
source_yaml_url: https://artifacts.apis.io/triplebooks-com/authentication/triplebooks-com-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Payroll
- Invoicing
- Cap table
- Multi‑entity
- API
- Finance automation
---
