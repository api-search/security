---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcp-openapi.yaml
  format: yaml
  label: LexLint API
  slug: lexlint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexlint-io/openapi/mcp-openapi.yaml
auth_types: []
description: LexLint authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LexLint Authentication
name_suffix: Authentication
oauth_flows: []
overview: LexLint declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LexLint
provider_slug: lexlint-io
scheme_count: 2
schemes:
- evidence: The key travels as the X-API-Key header on every request to mcp.lexlint.io , which passes it through to the UnGovr Open Data API on your behalf.
  header: X-API-Key
  how_to_obtain: Get a key via /lexlint:lexlint-key in a Claude Code session, claim_trial_key, or from https://lexlint.io/trial or an account at https://www.ungovr.org/open-data/api-keys.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Signing in gives the client an access token for your account, sent as Authorization: Bearer and metered on your account''s allowance like a key.'
  header: Authorization
  how_to_obtain: Sign in through ungovr.org to receive an OAuth access token.
  location: header
  name: Bearer
  type: http-bearer
slug: lexlint-io-authentication
source_filename: lexlint-io-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.lexlint.io/api-keys
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.lexlint.io/api-keys\nsources:\n- https://developer.lexlint.io/api-keys\n- https://developer.lexlint.io/quickstart\ndescription: LexLint authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: The key travels as the X-API-Key header on every request to mcp.lexlint.io , which passes it through to the UnGovr Open Data API on\n    your behalf.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get a key via /lexlint:lexlint-key in a Claude Code session, claim_trial_key, or from https://lexlint.io/trial or an account\n    at https://www.ungovr.org/open-data/api-keys.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Signing in gives the client an access token for your account, sent as Authorization: Bearer and metered on your account''s allowance\n    like a key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in through\
  \ ungovr.org to receive an OAuth access token.\ndocs: https://developer.lexlint.io/api-keys\n"
source_yaml_url: https://artifacts.apis.io/lexlint-io/authentication/lexlint-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Compliance
- Artificial Intelligence
- Privacy
- Cybersecurity
---
