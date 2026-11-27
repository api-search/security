---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ifrcoworker-app-openapi-generated.yml
  format: yaml
  label: ifrCoworker API
  slug: ifrcoworker-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ifrcoworker-app/openapi/_ae-authored/ifrcoworker-app-openapi-generated.yml
auth_types: []
description: Authentication methods as published on the provider page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ifrCoworker Authentication
name_suffix: Authentication
oauth_flows: []
overview: ifrCoworker declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ifrCoworker
provider_slug: ifrcoworker-app
scheme_count: 1
schemes:
- evidence: MCP over Streamable HTTP with the key as a Bearer header — any HTTP client
  header: Authorization
  how_to_obtain: Create an API key in the provider portal; the key is used as a Bearer token in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: ifrcoworker-app-authentication
source_filename: ifrcoworker-app-authentication.yml
source_heading: Authentication Profile
source_url: https://ifrcoworker.app/access
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ifrcoworker.app/access\nsources:\n- https://ifrcoworker.app/access\ndescription: Authentication methods as published on the provider page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: MCP over Streamable HTTP with the key as a Bearer header — any HTTP client\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the provider portal; the key is used as a Bearer token in the Authorization header.\ndocs: https://ifrcoworker.app/access\n"
source_yaml_url: https://artifacts.apis.io/ifrcoworker-app/authentication/ifrcoworker-app-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Artificial Intelligence
- Financial Reporting
- IFRS
- MCP
---
