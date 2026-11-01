---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published by Next Matter
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Next Matter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Next Matter declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Next Matter
provider_slug: next-matter
scheme_count: 5
schemes:
- evidence: Note that the initial authorization is done using the OAuth2 flow, and then we request additional scopes for each connected Microsoft service.
  name: Microsoft SSO
  type: oauth2
- evidence: You can log in to Next Matter using Okta
  name: Okta
  type: oauth2
- evidence: For API Key HTTP, Header Name is the HTTP header that carries the key. It defaults to `Authorization`. Change it when the API expects a different header, like `X-API-Key`. Prefix is optional. Use it when the API expects a scheme in front of the key, like `Bearer`.
  header: Authorization
  how_to_obtain: Create an API key in the Next Matter admin UI (Company > Next Matter API keys) and copy the generated key.
  location: header
  name: API Key HTTP
  type: apiKey
- evidence: 'Basic: username and password'
  header: Authorization
  how_to_obtain: Add a new Basic HTTP credential in the Automations library > Custom credentials.
  location: header
  name: Basic HTTP
  type: http-basic
- evidence: 'Bearer: token'
  header: Authorization
  how_to_obtain: Add a new Bearer HTTP credential in the Automations library > Custom credentials.
  location: header
  name: Bearer HTTP
  type: http-bearer
slug: next-matter-authentication
source_filename: next-matter-authentication.yml
source_heading: Authentication Profile
source_url: https://help.nextmatter.com/docs/authenticate-with-microsoft.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.nextmatter.com/docs/authenticate-with-microsoft.md\nsources:\n- https://help.nextmatter.com/docs/authenticate-with-microsoft.md\n- https://help.nextmatter.com/docs/okta-authentication.md\n- https://help.nextmatter.com/docs/api-keys.md\n- https://help.nextmatter.com/docs/api-keys\ndescription: Authentication methods published by Next Matter\nschemes:\n- type: oauth2\n  name: Microsoft SSO\n  evidence: Note that the initial authorization is done using the OAuth2 flow, and then we request additional scopes for each connected Microsoft\n    service.\n- type: oauth2\n  name: Okta\n  evidence: You can log in to Next Matter using Okta\n- type: apiKey\n  name: API Key HTTP\n  evidence: For API Key HTTP, Header Name is the HTTP header that carries the key. It defaults to `Authorization`. Change it when the API expects\n    a different header, like `X-API-Key`. Prefix is optional.\
  \ Use it when the API expects a scheme in front of the key, like `Bearer`.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Next Matter admin UI (Company > Next Matter API keys) and copy the generated key.\n- type: http-basic\n  name: Basic HTTP\n  evidence: 'Basic: username and password'\n  location: header\n  header: Authorization\n  how_to_obtain: Add a new Basic HTTP credential in the Automations library > Custom credentials.\n- type: http-bearer\n  name: Bearer HTTP\n  evidence: 'Bearer: token'\n  location: header\n  header: Authorization\n  how_to_obtain: Add a new Bearer HTTP credential in the Automations library > Custom credentials.\ndocs: https://help.nextmatter.com/docs/authenticate-with-microsoft.md\n"
source_yaml_url: https://artifacts.apis.io/next-matter/authentication/next-matter-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Automation
- Workflow
- Integration
- SaaS
---
