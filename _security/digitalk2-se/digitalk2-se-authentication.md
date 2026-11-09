---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Digitalk2 Se Authentication
name_suffix: Authentication
oauth_flows: []
overview: DigitalK2 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DigitalK2
provider_slug: digitalk2-se
scheme_count: 1
schemes:
- applies_to: https://mcp.digitalk2.se/mcp
  description: OAuth 2.1 with PKCE and dynamic client registration; the user signs in with their DigitalK2 account in the browser and approves the connection. No API key.
  dynamic_client_registration: true
  flows:
  - authorizationCode
  name: oauth2
  pkce: required
  quote: Inloggning OAuth 2.1 med PKCE och dynamisk klientregistrering. Ingen API-nyckel.
  sources:
  - https://www.digitalk2.se/mcp
  - https://github.com/digitalk2se/digitalk2-plugin
  type: oauth2
slug: digitalk2-se-authentication
source_filename: digitalk2-se-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://www.digitalk2.se/mcp\ndocs: https://www.digitalk2.se/mcp\nname: DigitalK2 authentication\nnote: DigitalK2 publishes no OpenAPI; the only programmatic surface is the remote MCP server. The auth profile is read from the MCP docs page and the first-party plugin README. Endpoints were not called.\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://mcp.digitalk2.se/mcp\n  description: OAuth 2.1 with PKCE and dynamic client registration; the user signs in with their DigitalK2 account in the browser and approves the connection. No API key.\n  flows: [authorizationCode]\n  pkce: required\n  dynamic_client_registration: true\n  quote: Inloggning OAuth 2.1 med PKCE och dynamisk klientregistrering. Ingen API-nyckel.\n  sources:\n  - https://www.digitalk2.se/mcp\n  - https://github.com/digitalk2se/digitalk2-plugin\napi_keys: false\ntoken_lifetime: \"Kortlivade inloggningar som förnyas automatiskt. (short-lived sign-ins\
  \ renewed automatically; no duration stated)\"\nrevocation: \"Koppla från när som helst, då slutar åtkomsten direkt. (disconnect at any time, access stops immediately)\"\n"
source_yaml_url: https://artifacts.apis.io/digitalk2-se/authentication/digitalk2-se-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Accounting
- Annual Reports
- Bolagsverket
- Sweden
- SIE
- Small Business
- Tax
- MCP
---
