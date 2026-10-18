---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fyrn-openapi-generated.yml
  format: yaml
  label: Fyrn API
  slug: fyrn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyrn/refs/heads/main/openapi/_ae-authored/fyrn-openapi-generated.yml
auth_types: []
description: Authentication methods for Fyrn CLI and API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fyrn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fyrn declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fyrn
provider_slug: fyrn
scheme_count: 2
schemes:
- evidence: This opens your browser for Auth0 PKCE authentication.
  flows:
  - authorization_code
  how_to_obtain: Run `fyrn login` which opens a browser for Auth0 PKCE authentication; on success credentials are stored in ~/.fyrn/credentials.json .
  name: Auth0 PKCE
  type: oauth2
- evidence: 'For headless environments, authenticate with an API key instead:'
  header: Authorization
  how_to_obtain: Run `fyrn auth api-key --api-key sk-your-key --api-url https://api.fyrn.dev` to store the API key in ~/.fyrn/config.json .
  location: header
  name: API key
  type: apiKey
slug: fyrn-authentication
source_filename: fyrn-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fyrn.ai/getting-started/
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fyrn.ai/getting-started/\nsources:\n- https://docs.fyrn.ai/getting-started/\n- https://docs.fyrn.ai/getting-started/installation/\n- https://docs.fyrn.ai/getting-started/quickstart/\ndescription: Authentication methods for Fyrn CLI and API\nschemes:\n- type: oauth2\n  name: Auth0 PKCE\n  evidence: This opens your browser for Auth0 PKCE authentication.\n  flows:\n  - authorization_code\n  how_to_obtain: Run `fyrn login` which opens a browser for Auth0 PKCE authentication; on success credentials are stored in ~/.fyrn/credentials.json\n    .\n- type: apiKey\n  name: API key\n  evidence: 'For headless environments, authenticate with an API key instead:'\n  location: header\n  header: Authorization\n  how_to_obtain: Run `fyrn auth api-key --api-key sk-your-key --api-url https://api.fyrn.dev` to store the API key in ~/.fyrn/config.json .\ndocs: https://docs.fyrn.ai/getting-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyrn/refs/heads/main/authentication/fyrn-authentication.yml
summary_line: 2 schemes
tags:
- Integration
- AI
- Automation
- Enterprise
- Platform
- Company
---
