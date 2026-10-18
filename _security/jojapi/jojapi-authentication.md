---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jojapi-openapi-generated.yml
  format: yaml
  label: APRYCO API
  slug: jojapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jojapi/refs/heads/main/openapi/_ae-authored/jojapi-openapi-generated.yml
auth_types: []
description: Authentication methods for JoJ API keys as documented on the JoJ API pages.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Jojapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: APRYCO declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: APRYCO
provider_slug: jojapi
scheme_count: 4
schemes:
- evidence: Send your API key via the custom `X-JoJAPI-Key` HTTP header.
  header: X-JoJAPI-Key
  location: header
  name: X-JoJAPI-Key Header
  type: apiKey
- evidence: Pass your API key directly through the `Authorization` header without any prefix.
  header: Authorization
  location: header
  name: Authorization Header (raw)
  type: apiKey
- evidence: Use the `Authorization` header with the `Bearer` scheme followed by your API key.
  header: Authorization
  location: header
  name: Bearer Token
  type: http-bearer
- evidence: 'Send your API key using HTTP Basic Authentication: the `Authorization` header contains the word `Basic`, followed by the base64 encoding of `YOUR_API_KEY:YOUR_API_KEY` — the key doubles as both username and password.'
  header: Authorization
  location: header
  name: Basic Token
  type: http-basic
slug: jojapi-authentication
source_filename: jojapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jojapi.com/consumers/api-keys.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jojapi.com/consumers/api-keys.md\nsources:\n- https://docs.jojapi.com/consumers/api-keys.md\n- https://docs.jojapi.com/account/two-factor-authentication.md\ndescription: Authentication methods for JoJ API keys as documented on the JoJ API pages.\nschemes:\n- type: apiKey\n  name: X-JoJAPI-Key Header\n  evidence: Send your API key via the custom `X-JoJAPI-Key` HTTP header.\n  location: header\n  header: X-JoJAPI-Key\n- type: apiKey\n  name: Authorization Header (raw)\n  evidence: Pass your API key directly through the `Authorization` header without any prefix.\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Bearer Token\n  evidence: Use the `Authorization` header with the `Bearer` scheme followed by your API key.\n  location: header\n  header: Authorization\n- type: http-basic\n  name: Basic Token\n  evidence: 'Send your API key using HTTP\
  \ Basic Authentication: the `Authorization` header contains the word `Basic`, followed by the base64 encoding\n    of `YOUR_API_KEY:YOUR_API_KEY` — the key doubles as both username and password.'\n  location: header\n  header: Authorization\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other authentication schemes are described on the provided pages.\ndocs: https://docs.jojapi.com/consumers/api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jojapi/refs/heads/main/authentication/jojapi-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Marketplace
- Data
- Scraping
- APIs
---
