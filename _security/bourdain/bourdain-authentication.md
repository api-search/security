---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bourdain-openapi-generated.yml
  format: yaml
  label: Bourdain API
  slug: bourdain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bourdain/refs/heads/main/openapi/_ae-authored/bourdain-openapi-generated.yml
auth_types: []
description: Bourdain uses API keys passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bourdain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bourdain declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bourdain
provider_slug: bourdain
scheme_count: 1
schemes:
- evidence: All API requests must include an Authorization header with your API key as a Bearer token.
  header: Authorization
  how_to_obtain: Generate API keys from your account settings (Settings → API Keys).
  location: header
  name: Authorization
  scopes:
  - acp_read
  - acp_purchase
  - mcp_tools
  - webhooks
  type: apiKey
slug: bourdain-authentication
source_filename: bourdain-authentication.yml
source_heading: Authentication Profile
source_url: https://www.bourdain.io/docs/authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.bourdain.io/docs/authentication\nsources:\n- https://www.bourdain.io/docs/authentication\n- https://www.bourdain.io/docs/getting-started\n- https://www.bourdain.io/docs/quickstart\n- https://www.bourdain.io/seller/onboarding\ndescription: Bourdain uses API keys passed as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: All API requests must include an Authorization header with your API key as a Bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - acp_read\n  - acp_purchase\n  - mcp_tools\n  - webhooks\n  how_to_obtain: Generate API keys from your account settings (Settings → API Keys).\nnote: No OAuth2, HTTP Basic, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://www.bourdain.io/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bourdain/refs/heads/main/authentication/bourdain-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketplace
- Trading Cards
- AI
- E-commerce
- Collectibles
---
