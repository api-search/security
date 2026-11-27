---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aitrips.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aitrips.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Aitrips.io
provider_slug: aitrips-io
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 with PKCE, token issued by aitrips.io (dynamic client registration supported)
  flows:
    authorizationCode:
      authorizationUrl: https://www.aitrips.io/oauth/authorize
      scopes: {}
      tokenUrl: https://www.aitrips.io/oauth/token
  type: oauth2
- description: API key fallback for clients that cannot run OAuth flow
  in: header
  name: X-API-Key
  type: apiKey
slug: aitrips-io-authentication
source_filename: aitrips-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://www.aitrips.io/docs\nschemes:\n  - type: oauth2\n    description: OAuth 2.0 with PKCE, token issued by aitrips.io (dynamic client registration supported)\n    bearerFormat: JWT\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.aitrips.io/oauth/authorize\n        tokenUrl: https://www.aitrips.io/oauth/token\n        scopes: {}\n  - type: apiKey\n    description: API key fallback for clients that cannot run OAuth flow\n    name: X-API-Key\n    in: header\n"
source_yaml_url: https://artifacts.apis.io/aitrips-io/authentication/aitrips-io-authentication.yml
summary_line: 2 schemes
tags:
- Travel
- Mapping
- Trip Planning
- Artificial Intelligence
- Transportation
- Weather
---
