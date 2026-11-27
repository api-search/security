---
anonymous_access: false
api_key_in: []
api_specs:
- filename: membase-ai-agent-protocol-api-openapi.yml
  format: yaml
  label: Membase Agent Protocol API
  slug: membase-ai-agent-protocol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/membase-ai/openapi/membase-ai-agent-protocol-api-openapi.yml
auth_types: []
description: Authentication & Scopes Every call carries a bearer.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Membase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Membase declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Membase
provider_slug: membase-ai
scheme_count: 1
schemes:
- evidence: 'Every request to https://api.app.membase.com carries one header: Authorization: Bearer <credential>'
  header: Authorization
  how_to_obtain: Minted by the account’s owner under Connect › Developer keys or approved via the OAuth consent screen.
  location: header
  name: Bearer token
  type: http-bearer
slug: membase-ai-authentication
source_filename: membase-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.membase.com/build/reference/authentication/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.membase.com/build/reference/authentication/\nsources:\n- https://docs.membase.com/build/reference/authentication/\n- https://docs.membase.com/use/getting-started/quickstart/\n- https://docs.membase.com/use/getting-started/sign-in/\n- https://docs.membase.com/use/getting-started/first-run-guide/\ndescription: Authentication & Scopes Every call carries a bearer.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every request to https://api.app.membase.com carries one header: Authorization: Bearer <credential>'\n  location: header\n  header: Authorization\n  how_to_obtain: Minted by the account’s owner under Connect › Developer keys or approved via the OAuth consent screen.\ndocs: https://docs.membase.com/build/reference/authentication/\n"
source_yaml_url: https://artifacts.apis.io/membase-ai/authentication/membase-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Platform
- Developer Tools
- Unibase
---
