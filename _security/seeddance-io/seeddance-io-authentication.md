---
anonymous_access: false
api_key_in: []
auth_types: []
description: SeedVideo AI API uses API keys provided as a Bearer token in the Authorization header of every request.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: SeedVideo AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: SeedVideo AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SeedVideo AI
provider_slug: seeddance-io
scheme_count: 1
schemes:
- evidence: Include a SeedVideo AI API key in the HTTP Bearer header of every /v1 request.
  header: Authorization
  how_to_obtain: Create a key in Settings → API keys, copy the secret once, and store it securely on the server.
  location: header
  name: Authorization
  type: http-bearer
slug: seeddance-io-authentication
source_filename: seeddance-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.seeddance.io/docs/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.seeddance.io/docs/authentication\nsources:\n- https://www.seeddance.io/docs/authentication\n- https://www.seeddance.io/docs\ndescription: SeedVideo AI API uses API keys provided as a Bearer token in the Authorization header of every request.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Include a SeedVideo AI API key in the HTTP Bearer header of every /v1 request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → API keys, copy the secret once, and store it securely on the server.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://www.seeddance.io/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/seeddance-io/authentication/seeddance-io-authentication.yml
summary_line: 1 scheme
tags:
- AI Video Generation
- Video Generation
- Image-to-Video
- Creative Tools
---
