---
anonymous_access: false
api_key_in: []
auth_types: []
description: Maguyva authenticates requests using an API key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Maguyva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maguyva declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Maguyva
provider_slug: maguyva-tools
scheme_count: 2
schemes:
- evidence: 'Every request authenticates with your API key, sent as an Authorization: Bearer header or, where a client cannot set one, an X-API-Key header.'
  header: Authorization
  how_to_obtain: Obtain the API key (it starts with mgv_) from app.maguyva.ai.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Every request authenticates with your API key, sent as an Authorization: Bearer header or, where a client cannot set one, an X-API-Key header.'
  header: X-API-Key
  how_to_obtain: Obtain the API key (it starts with mgv_) from app.maguyva.ai.
  location: header
  name: X-API-Key header
  type: apiKey
slug: maguyva-tools-authentication
source_filename: maguyva-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://maguyva.ai/docs/troubleshooting
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://maguyva.ai/docs/troubleshooting\nsources:\n- https://maguyva.ai/docs/troubleshooting\n- https://maguyva.ai/docs/quickstart.md\n- https://maguyva.ai/docs/quickstart\n- https://maguyva.ai/ar/docs/quickstart\ndescription: Maguyva authenticates requests using an API key.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every request authenticates with your API key, sent as an Authorization: Bearer header or, where a client cannot set one, an X-API-Key\n    header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the API key (it starts with mgv_) from app.maguyva.ai.\n- type: apiKey\n  name: X-API-Key header\n  evidence: 'Every request authenticates with your API key, sent as an Authorization: Bearer header or, where a client cannot set one, an X-API-Key\n    header.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Obtain the\
  \ API key (it starts with mgv_) from app.maguyva.ai.\nnote: No OAuth2, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://maguyva.ai/docs/troubleshooting\n"
source_yaml_url: https://artifacts.apis.io/maguyva-tools/authentication/maguyva-tools-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Tools
- MCP
- Serverless
- Cloudflare
---
