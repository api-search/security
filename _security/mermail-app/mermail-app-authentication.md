---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mermail-app-agent-api-openapi.yml
  format: yaml
  label: Mermail Agent API
  slug: mermail-app-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mermail-app/openapi/mermail-app-agent-api-openapi.yml
- filename: mermail-app-mermail-agent-marketplace-api-openapi.yml
  format: yaml
  label: Mermail Mermail Agent Marketplace API
  slug: mermail-app-mermail-agent-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mermail-app/openapi/mermail-app-mermail-agent-marketplace-api-openapi.yml
auth_types: []
description: Mermail uses a workspace‑scoped API key sent in the request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mermail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mermail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mermail
provider_slug: mermail-app
scheme_count: 1
schemes:
- evidence: Authenticate sold API calls with a Mermail API key via x-api-key.
  header: x-api-key
  how_to_obtain: Create a key in Settings → API Keys; copy the key once.
  location: header
  name: apiKey
  type: apiKey
slug: mermail-app-authentication
source_filename: mermail-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mermail.app/api-reference/authentication.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mermail.app/api-reference/authentication.md\nsources:\n- https://docs.mermail.app/api-reference/authentication.md\n- https://docs.mermail.app/agent-wallet/catalog-transfers.md\n- https://docs.mermail.app/api-reference/webhooks/rotate-signing-secret.md\n- https://docs.mermail.app/api-reference/rag/get-rag-credentials-status.md\ndescription: Mermail uses a workspace‑scoped API key sent in the request header.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Authenticate sold API calls with a Mermail API key via x-api-key.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key in Settings → API Keys; copy the key once.\nnote: No OAuth2, http‑basic, http‑bearer, JWT, HMAC, MTLS, or other schemes are documented.\ndocs: https://docs.mermail.app/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/mermail-app/authentication/mermail-app-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Artificial Intelligence
- Wallets
- Automation
---
