---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lazaretto-dev-attestations-api-openapi.yml
  format: yaml
  label: Lazaretto Attestations API
  slug: lazaretto-dev-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-attestations-api-openapi.yml
- filename: lazaretto-dev-benchmark-json-api-openapi.yml
  format: yaml
  label: Lazaretto Benchmark.json API
  slug: lazaretto-dev-benchmark-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-benchmark-json-api-openapi.yml
- filename: lazaretto-dev-check-api-openapi.yml
  format: yaml
  label: Lazaretto Check API
  slug: lazaretto-dev-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-check-api-openapi.yml
- filename: lazaretto-dev-checkout-api-openapi.yml
  format: yaml
  label: Lazaretto Checkout API
  slug: lazaretto-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-checkout-api-openapi.yml
- filename: lazaretto-dev-credits-api-openapi.yml
  format: yaml
  label: Lazaretto Credits API
  slug: lazaretto-dev-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-credits-api-openapi.yml
- filename: lazaretto-dev-health-api-openapi.yml
  format: yaml
  label: Lazaretto Health API
  slug: lazaretto-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-health-api-openapi.yml
- filename: lazaretto-dev-known-bad-api-openapi.yml
  format: yaml
  label: Lazaretto Known Bad API
  slug: lazaretto-dev-known-bad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-known-bad-api-openapi.yml
- filename: lazaretto-dev-lockfile-api-openapi.yml
  format: yaml
  label: Lazaretto Lockfile API
  slug: lazaretto-dev-lockfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-lockfile-api-openapi.yml
- filename: lazaretto-dev-mcp-api-openapi.yml
  format: yaml
  label: Lazaretto MCP API
  slug: lazaretto-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-mcp-api-openapi.yml
- filename: lazaretto-dev-rules-api-openapi.yml
  format: yaml
  label: Lazaretto Rules API
  slug: lazaretto-dev-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-rules-api-openapi.yml
- filename: lazaretto-dev-scan-api-openapi.yml
  format: yaml
  label: Lazaretto Scan API
  slug: lazaretto-dev-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-scan-api-openapi.yml
- filename: lazaretto-dev-trial-api-openapi.yml
  format: yaml
  label: Lazaretto Trial API
  slug: lazaretto-dev-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-trial-api-openapi.yml
- filename: lazaretto-dev-usage-api-openapi.yml
  format: yaml
  label: Lazaretto Usage API
  slug: lazaretto-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-usage-api-openapi.yml
- filename: lazaretto-dev-verify-api-openapi.yml
  format: yaml
  label: Lazaretto Verify API
  slug: lazaretto-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-verify-api-openapi.yml
- filename: lazaretto-dev-watch-api-openapi.yml
  format: yaml
  label: Lazaretto Watch API
  slug: lazaretto-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-watch-api-openapi.yml
- filename: lazaretto-dev-well-known-api-openapi.yml
  format: yaml
  label: Lazaretto .well Known API
  slug: lazaretto-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-well-known-api-openapi.yml
auth_types: []
description: Lazaretto connectors generally use no authentication, but some CLI tools allow an optional API key sent in the X-API-Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lazaretto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lazaretto declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lazaretto
provider_slug: lazaretto-dev
scheme_count: 2
schemes:
- evidence: 'Add a key for the scans that read code In Gemini CLI, put the key itself in the command: gemini mcp add --transport http --scope user --header "X-API-Key: YOUR_KEY" lazaretto "https://lazaretto.dev/mcp?ref=gemini"'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Select + , then Add custom MCP server . Name it Lazaretto and paste https://lazaretto.dev/mcp/connector as the server URL. Set authentication to No authentication , tick I understand and want to continue , and select Create as a plugin .
  name: No authentication
  type: other
slug: lazaretto-dev-authentication
source_filename: lazaretto-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://lazaretto.dev/.well-known/jwks.json
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lazaretto.dev/.well-known/jwks.json\nsources:\n- https://lazaretto.dev/.well-known/jwks.json\n- https://lazaretto.dev/add\ndescription: Lazaretto connectors generally use no authentication, but some CLI tools allow an optional API key sent in the X-API-Key header.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Add a key for the scans that read code In Gemini CLI, put the key itself in the command: gemini mcp add --transport http --scope\n    user --header \"X-API-Key: YOUR_KEY\" lazaretto \"https://lazaretto.dev/mcp?ref=gemini\"'\n  location: header\n  header: X-API-Key\n- type: other\n  name: No authentication\n  evidence: Select + , then Add custom MCP server . Name it Lazaretto and paste https://lazaretto.dev/mcp/connector as the server URL. Set authentication\n    to No authentication , tick I understand and want to continue , and select Create as a plugin\
  \ .\ndocs: https://lazaretto.dev/.well-known/jwks.json\n"
source_yaml_url: https://artifacts.apis.io/lazaretto-dev/authentication/lazaretto-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- npm
- Malware
- Open Source
---
