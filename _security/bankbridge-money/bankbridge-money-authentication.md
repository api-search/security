---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bankbridge-money-openapi-generated.yml
  format: yaml
  label: BankBridge API
  slug: bankbridge-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankbridge-money/openapi/_ae-authored/bankbridge-money-openapi-generated.yml
auth_types: []
description: Authentication methods for BankBridge as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bankbridge Money Authentication
name_suffix: Authentication
oauth_flows: []
overview: BankBridge declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BankBridge
provider_slug: bankbridge-money
scheme_count: 2
schemes:
- evidence: Check the Authorization header starts with `Bearer ` (note the space) and ends in a key you still own.
  header: Authorization
  how_to_obtain: Copy the API key from Settings after rotating and paste it into the Authorization header as a Bearer token.
  location: header
  name: Bearer
  type: http-bearer
- evidence: ChatGPT opens a BankBridge sign‑in window. Enter your email, click the magic link, then **Allow** back in ChatGPT. No API key to copy, no token to paste.
  how_to_obtain: Sign in via the BankBridge OAuth flow in ChatGPT or Claude connectors; no token is pasted.
  name: OAuth
  type: oauth2
slug: bankbridge-money-authentication
source_filename: bankbridge-money-authentication.yml
source_heading: Authentication Profile
source_url: https://bankbridge.money/guides/how-to-rotate-your-bankbridge-api-key
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bankbridge.money/guides/how-to-rotate-your-bankbridge-api-key\nsources:\n- https://bankbridge.money/guides/how-to-rotate-your-bankbridge-api-key\n- https://bankbridge.money/docs/chatgpt-apps-sdk.md\n- https://bankbridge.money/guides/how-to-rotate-your-bankbridge-api-key.md\n- https://bankbridge.money/docs/claude-web\ndescription: Authentication methods for BankBridge as documented.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Check the Authorization header starts with `Bearer ` (note the space) and ends in a key you still own.\n  location: header\n  header: Authorization\n  how_to_obtain: Copy the API key from Settings after rotating and paste it into the Authorization header as a Bearer token.\n- type: oauth2\n  name: OAuth\n  evidence: ChatGPT opens a BankBridge sign‑in window. Enter your email, click the magic link, then **Allow** back in ChatGPT. No API\
  \ key to copy,\n    no token to paste.\n  how_to_obtain: Sign in via the BankBridge OAuth flow in ChatGPT or Claude connectors; no token is pasted.\ndocs: https://bankbridge.money/guides/how-to-rotate-your-bankbridge-api-key\n"
source_yaml_url: https://artifacts.apis.io/bankbridge-money/authentication/bankbridge-money-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- AI
- MCP
- Banking
---
