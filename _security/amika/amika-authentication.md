---
api_key_in:
- header
api_specs:
- filename: amika-openapi.json
  format: json
  label: Amika API
  slug: amika-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-openapi.json
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Amika Authentication
name_suffix: Authentication
oauth_flows:
- deviceAuthorization
overview: Amika secures its APIs with http, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceAuthorization flow(s).
provider_name: Amika
provider_slug: amika
scheme_count: 4
schemes:
- description: 'Bearer token in the Authorization header. The token is either a long-lived API key created in the web UI (app.amika.dev/settings) or a short-lived access token minted by the OAuth device-authorization login flow. The CLI resolves credentials in precedence order: AMIKA_API_KEY env var, stored API key file (${XDG_STATE_HOME}/amika/api-key.json), then browser login session.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.amika.dev/reference/auth
  type: http
- description: API keys generated in the web UI for non-interactive/CI use. Provided via the AMIKA_API_KEY environment variable or on-disk key file, presented as a bearer token to the API. Managed through the /api-keys operations.
  in: header
  name: apiKey
  sources:
  - https://docs.amika.dev/reference/auth
  type: apiKey
- description: Interactive browser login for local development. The CLI requests a device code, the user authorizes in the browser, the CLI polls until complete, and a session is stored with access token, refresh token, email, and org. Tokens auto-refresh within 60 seconds of expiry. Identity is brokered by WorkOS.
  flow: deviceAuthorization
  name: deviceAuthorization
  sources:
  - https://docs.amika.dev/reference/auth
  type: oauth2
- description: Session cookie accepted for browser-originated (web app) requests, offered as an alternative to bearerAuth on every operation.
  in: cookie
  name: cookieAuth
  sources:
  - openapi/amika-openapi.json
  type: apiKey
slug: amika-authentication
source_filename: amika-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.amika.dev/reference/auth.md\ndocs: https://docs.amika.dev/reference/auth\nsummary:\n  types: [http, apiKey, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [deviceAuthorization]\n  notes: >-\n    The OpenAPI declares two security requirements per operation (bearerAuth and\n    cookieAuth) but does not define them under components.securitySchemes. The\n    profile below is reconstructed from the published authentication docs.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token in the Authorization header. The token is either a long-lived\n    API key created in the web UI (app.amika.dev/settings) or a short-lived\n    access token minted by the OAuth device-authorization login flow. The CLI\n    resolves credentials in precedence order: AMIKA_API_KEY env var, stored API\n    key file (${XDG_STATE_HOME}/amika/api-key.json), then browser login\
  \ session.\n  sources: [https://docs.amika.dev/reference/auth]\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    API keys generated in the web UI for non-interactive/CI use. Provided via\n    the AMIKA_API_KEY environment variable or on-disk key file, presented as a\n    bearer token to the API. Managed through the /api-keys operations.\n  sources: [https://docs.amika.dev/reference/auth]\n- name: deviceAuthorization\n  type: oauth2\n  flow: deviceAuthorization\n  description: >-\n    Interactive browser login for local development. The CLI requests a device\n    code, the user authorizes in the browser, the CLI polls until complete, and\n    a session is stored with access token, refresh token, email, and org.\n    Tokens auto-refresh within 60 seconds of expiry. Identity is brokered by\n    WorkOS.\n  sources: [https://docs.amika.dev/reference/auth]\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  description: >-\n    Session cookie accepted for browser-originated\
  \ (web app) requests, offered\n    as an alternative to bearerAuth on every operation.\n  sources: [openapi/amika-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/authentication/amika-authentication.yml
summary_line: http/apiKey/oauth2 · 4 schemes
tags:
- Company
- AI Agents
- Coding Agents
- Developer Tools
- Sandboxes
- Infrastructure
- CI/CD
- Automation
- Software Factory
- API
---
