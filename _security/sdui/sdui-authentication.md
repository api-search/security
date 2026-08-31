---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sdui Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sdui declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Sdui
provider_slug: sdui
scheme_count: 0
schemes: []
slug: sdui-authentication
source_filename: sdui-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live unauthenticated probes of https://api.sdui.app/v1/* and https://sdui.de/.well-known/*\ndocs: null\ndocs_note: >-\n  Sdui publishes no authentication documentation. There is no developer portal, no API reference and\n  no page in the sdui.de sitemap (176 pages walked) describing credentials, tokens or key issuance.\n  Everything below is observed from live unauthenticated responses, not from provider prose.\napis:\n- api: Sdui Platform API\n  base_url: https://api.sdui.app/v1\n  schemes:\n  - type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    evidence:\n      url: https://api.sdui.app/v1/\n      http_status: 404\n      response_header: 'www-authenticate: Bearer'\n    note: >-\n      The server emits `WWW-Authenticate: Bearer` on unauthenticated requests. Protected resources\n      answer HTTP 401 with the envelope\n      {\"data\":[],\"status\":\"ERROR\",\"meta\":{\"errors\":[\"Bitte zuerst einloggen.\"\
  ]}} — German for\n      \"Please log in first\". The token issuance flow is not publicly documented; credentials are\n      obtained by signing in to a school tenant in the Sdui app, or through the partner/sales channel\n      for integrations such as the WebUntis messenger.\n  oauth2: false\n  api_key: false\n  mtls: false\n  gated: true\n- api: Sdui Website MCP Server\n  base_url: https://sdui.de/wp-json/mcp\n  schemes:\n  - type: oauth2\n    flow: authorization_code\n    pkce: S256\n    authorization_endpoint: https://sdui.de/oauth/authorize\n    token_endpoint: https://sdui.de/oauth/token\n    revocation_endpoint: https://sdui.de/oauth/revoke\n    scopes: [mcp]\n    token_endpoint_auth_methods: [none]\n    evidence:\n      url: https://sdui.de/.well-known/oauth-authorization-server\n      http_status: 200\n  oauth2: true\n  api_key: false\n  mtls: false\n  gated: true\nsummary:\n  auth_documented: false\n  discovery_document_present: true\n  discovery_document_scope: MCP server on\
  \ the WordPress site only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sdui/refs/heads/main/authentication/sdui-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Education
- EdTech
- Schools
- Communications
- Messaging
- Timetabling
- Grade Management
- Germany
- GDPR
---
