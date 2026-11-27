---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datagalactica-com-api-openapi.json
  format: json
  label: Data Galactica API API
  slug: data-galactica-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagalactica-com/openapi/_original/datagalactica-com-api-openapi.json
auth_types: []
description: Data Galactica supports OAuth 2.1 authorization code flow with PKCE and API keys sent as Bearer tokens or X-API-Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Data Galactica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Data Galactica declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Data Galactica
provider_slug: datagalactica-com
scheme_count: 2
schemes:
- evidence: Agents should authenticate with OAuth 2.1, the person approving in a browser, or, when no browser is available, through an e-mail code the person reads out.
  flows:
  - authorization_code
  how_to_obtain: Client registers at /oauth/register (public clients, no secret) and runs authorization code flow with PKCE (S256).
  name: OAuth 2.1
  type: oauth2
- evidence: Send the key in the Authorization header as a bearer token. X-API-Key also works, and on api.datagalactica.com so does Ocp-Apim-Subscription-Key.
  header: Authorization
  how_to_obtain: Sign up at /signup, receive a 6‑digit code via e‑mail, claim it at /agent/identity/claim to receive an API key.
  location: header
  name: API Key
  type: http-bearer
slug: datagalactica-com-authentication
source_filename: datagalactica-com-authentication.yml
source_heading: Authentication Profile
source_url: https://datagalactica.com/blog/agent-ready-data-api
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datagalactica.com/blog/agent-ready-data-api\nsources:\n- https://datagalactica.com/blog/agent-ready-data-api\n- https://datagalactica.com/blog/data-galactica-api-quickstart\n- https://datagalactica.com/blog/kyb-vendor-verification-api\ndescription: Data Galactica supports OAuth 2.1 authorization code flow with PKCE and API keys sent as Bearer tokens or X-API-Key header.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Agents should authenticate with OAuth 2.1, the person approving in a browser, or, when no browser is available, through an e-mail\n    code the person reads out.\n  flows:\n  - authorization_code\n  how_to_obtain: Client registers at /oauth/register (public clients, no secret) and runs authorization code flow with PKCE (S256).\n- type: http-bearer\n  name: API Key\n  evidence: Send the key in the Authorization header as a bearer token. X-API-Key also\
  \ works, and on api.datagalactica.com so does Ocp-Apim-Subscription-Key.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at /signup, receive a 6‑digit code via e‑mail, claim it at /agent/identity/claim to receive an API key.\ndocs: https://datagalactica.com/blog/agent-ready-data-api\n"
source_yaml_url: https://artifacts.apis.io/datagalactica-com/authentication/datagalactica-com-authentication.yml
summary_line: 2 schemes
tags:
- Data
- Identity
- Registry
- Prospecting
---
