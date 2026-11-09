---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blvigil-com-agent-api-openapi.yml
  format: yaml
  label: Vigil Agent API
  slug: blvigil-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvigil-com/openapi/blvigil-com-agent-api-openapi.yml
- filename: blvigil-com-mcp-api-openapi.yml
  format: yaml
  label: Vigil MCP API
  slug: blvigil-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvigil-com/openapi/blvigil-com-mcp-api-openapi.yml
auth_types: []
description: Authentication uses an API key that is sent as a Bearer token in the Authorization header or embedded in the URL.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Blvigil Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vigil declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Vigil
provider_slug: blvigil-com
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer ace_sk_YOUR_KEY'
  header: Authorization
  how_to_obtain: Sign in to get a key. Keys belong to your Ace account and reach the apps you connect.
  location: header
  name: API Key
  type: apiKey
- evidence: https://tryacee.com/mcp/k/ace_sk_YOUR_KEY
  how_to_obtain: Sign in to get a key. Keys belong to your Ace account and reach the apps you connect.
  location: query
  name: API Key (URL)
  type: apiKey
slug: blvigil-com-authentication
source_filename: blvigil-com-authentication.yml
source_heading: Authentication Profile
source_url: https://tryacee.com/developers?utm_source=blvigil.com&utm_medium=integrations&utm_campaign=platform-20261016
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tryacee.com/developers?utm_source=blvigil.com&utm_medium=integrations&utm_campaign=platform-20261016\nsources:\n- https://tryacee.com/developers?utm_source=blvigil.com&utm_medium=integrations&utm_campaign=platform-20261016\n- https://blvigil.com/resources/topics/setup/\n- https://blvigil.com/learn/one-room-setup/\ndescription: Authentication uses an API key that is sent as a Bearer token in the Authorization header or embedded in the URL.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Authorization: Bearer ace_sk_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to get a key. Keys belong to your Ace account and reach the apps you connect.\n- type: apiKey\n  name: API Key (URL)\n  evidence: https://tryacee.com/mcp/k/ace_sk_YOUR_KEY\n  location: query\n  how_to_obtain: Sign in to get a key. Keys belong to your Ace account and reach\
  \ the apps you connect.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented on the provided pages.\ndocs: https://tryacee.com/developers?utm_source=blvigil.com&utm_medium=integrations&utm_campaign=platform-20261016\n"
source_yaml_url: https://artifacts.apis.io/blvigil-com/authentication/blvigil-com-authentication.yml
summary_line: 2 schemes
tags:
- Home Automation
- Security
- Smart Home
- Software
- Mac
- Windows
---
