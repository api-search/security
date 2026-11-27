---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gnosismemory-com-openapi-generated.yml
  format: yaml
  label: Gnosis Memory API
  slug: gnosismemory-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosismemory-com/openapi/_ae-authored/gnosismemory-com-openapi-generated.yml
auth_types: []
description: OAuth 2.0 authorization code flow with Google, resulting in a bearer token placed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gnosis Memory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gnosis Memory declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gnosis Memory
provider_slug: gnosismemory-com
scheme_count: 1
schemes:
- evidence: Authenticate → Complete OAuth in your browser to get your token.
  header: Authorization
  how_to_obtain: User completes Google OAuth sign‑in in the browser; the service returns a bearer token that the client stores and sends as the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: gnosismemory-com-authentication
source_filename: gnosismemory-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gnosismemory.com/setup
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gnosismemory.com/setup\nsources:\n- https://gnosismemory.com/setup\ndescription: OAuth 2.0 authorization code flow with Google, resulting in a bearer token placed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authenticate → Complete OAuth in your browser to get your token.\n  location: header\n  header: Authorization\n  how_to_obtain: User completes Google OAuth sign‑in in the browser; the service returns a bearer token that the client stores and sends as the\n    Authorization header.\ndocs: https://gnosismemory.com/setup\n"
source_yaml_url: https://artifacts.apis.io/gnosismemory-com/authentication/gnosismemory-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Encryption
- Cross-Platform
- Developer Tools
- Company
---
