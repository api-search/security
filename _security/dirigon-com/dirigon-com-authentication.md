---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dirigon-com-openapi-generated.yml
  format: yaml
  label: Dirigon API
  slug: dirigon-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dirigon-com/openapi/_ae-authored/dirigon-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Dirigon API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dirigon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dirigon declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dirigon
provider_slug: dirigon-com
scheme_count: 2
schemes:
- evidence: 'Header: X-API-KEY .'
  header: X-API-KEY
  how_to_obtain: Get an API key on https://dirigon.com/billing and copy the secret; it is shown only once.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Interactive hosts (Claude, Cursor, ChatGPT, Grok, Claude Code): OAuth via https://dirigon.com/connect .'
  how_to_obtain: Use the OAuth flow at https://dirigon.com/connect for interactive hosts.
  name: OAuth
  type: oauth2
slug: dirigon-com-authentication
source_filename: dirigon-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dirigon.com/billing
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dirigon.com/billing\nsources:\n- https://dirigon.com/billing\n- https://dirigon.com/docs/quickstart.md\n- https://dirigon.com/docs/quickstart\ndescription: Authentication methods for Dirigon API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Header: X-API-KEY .'\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Get an API key on https://dirigon.com/billing and copy the secret; it is shown only once.\n- type: oauth2\n  name: OAuth\n  evidence: 'Interactive hosts (Claude, Cursor, ChatGPT, Grok, Claude Code): OAuth via https://dirigon.com/connect .'\n  how_to_obtain: Use the OAuth flow at https://dirigon.com/connect for interactive hosts.\ndocs: https://dirigon.com/billing\n"
source_yaml_url: https://artifacts.apis.io/dirigon-com/authentication/dirigon-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Credit
- Data
- SEC
---
