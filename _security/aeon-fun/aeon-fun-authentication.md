---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aeon-fun-api-openapi.json
  format: json
  label: aeon agent-facing API API
  slug: aeon-agent-facing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aeon-fun/openapi/_original/aeon-fun-api-openapi.json
auth_types: []
description: Authentication methods published across Aeon documentation pages.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Aeon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aeon declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Aeon
provider_slug: aeon-fun
scheme_count: 4
schemes:
- evidence: 'Have clients send keys in a header ( Authorization: Bearer , x-api-key or x-goog-api-key ) instead of the query string.'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Have clients send keys in a header ( Authorization: Bearer , x-api-key or x-goog-api-key ) instead of the query string. ds2api accepts all three.'
  header: x-api-key
  location: header
  name: API key
  type: apiKey
- evidence: 'Have clients send keys in a header ( Authorization: Bearer , x-api-key or x-goog-api-key ) instead of the query string. ds2api accepts all three.'
  header: x-goog-api-key
  location: header
  name: API key (Google style)
  type: apiKey
- authorize_url: https://www.aeon.fun/connect/oauth/authorize
  evidence: 'The flow is standard OAuth 2.1: discover, register a client, send the user to approve, exchange the code, then call the server with a Bearer token.'
  header: Authorization
  how_to_obtain: Register a client via dynamic registration or client metadata document, then perform the authorization code grant with PKCE to obtain an access token.
  location: header
  name: Aeon Connect OAuth 2.1
  scopes:
  - aeon
  - offline_access
  token_url: https://www.aeon.fun/connect/oauth/token
  type: oauth2
slug: aeon-fun-authentication
source_filename: aeon-fun-authentication.yml
source_heading: Authentication Profile
source_url: https://www.aeon.fun/security/advisories/ds2api-webui-path-traversal-api-key-logging
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.aeon.fun/security/advisories/ds2api-webui-path-traversal-api-key-logging\nsources:\n- https://www.aeon.fun/security/advisories/ds2api-webui-path-traversal-api-key-logging\n- https://www.aeon.fun/docs/auth\n- https://www.aeon.fun/auth.md\n- https://www.aeon.fun/security/advisories/openhuman-telegram-auth-csrf-session-implantation\ndescription: Authentication methods published across Aeon documentation pages.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Have clients send keys in a header ( Authorization: Bearer , x-api-key or x-goog-api-key ) instead of the query string.'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: API key\n  evidence: 'Have clients send keys in a header ( Authorization: Bearer , x-api-key or x-goog-api-key ) instead of the query string. ds2api accepts\n    all three.'\n  location: header\n  header: x-api-key\n\
  - type: apiKey\n  name: API key (Google style)\n  evidence: 'Have clients send keys in a header ( Authorization: Bearer , x-api-key or x-goog-api-key ) instead of the query string. ds2api accepts\n    all three.'\n  location: header\n  header: x-goog-api-key\n- type: oauth2\n  name: Aeon Connect OAuth 2.1\n  evidence: 'The flow is standard OAuth 2.1: discover, register a client, send the user to approve, exchange the code, then call the server with\n    a Bearer token.'\n  location: header\n  header: Authorization\n  token_url: https://www.aeon.fun/connect/oauth/token\n  authorize_url: https://www.aeon.fun/connect/oauth/authorize\n  scopes:\n  - aeon\n  - offline_access\n  how_to_obtain: Register a client via dynamic registration or client metadata document, then perform the authorization code grant with PKCE to\n    obtain an access token.\ndocs: https://www.aeon.fun/security/advisories/ds2api-webui-path-traversal-api-key-logging\n"
source_yaml_url: https://artifacts.apis.io/aeon-fun/authentication/aeon-fun-authentication.yml
summary_line: 4 schemes
tags:
- Artificial Intelligence
- Automation
- Open Source
- Framework
- Enterprise
---
