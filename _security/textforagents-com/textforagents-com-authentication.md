---
anonymous_access: false
api_key_in: []
api_specs:
- filename: textforagents-com-accounts-api-openapi.yml
  format: yaml
  label: textforagents-com Accounts API
  slug: textforagents-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-accounts-api-openapi.yml
- filename: textforagents-com-admin-api-openapi.yml
  format: yaml
  label: textforagents-com Admin API
  slug: textforagents-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-admin-api-openapi.yml
- filename: textforagents-com-auth-api-openapi.yml
  format: yaml
  label: textforagents-com Auth API
  slug: textforagents-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-auth-api-openapi.yml
- filename: textforagents-com-billing-api-openapi.yml
  format: yaml
  label: textforagents-com Billing API
  slug: textforagents-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-billing-api-openapi.yml
- filename: textforagents-com-health-api-openapi.yml
  format: yaml
  label: textforagents-com Health API
  slug: textforagents-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-health-api-openapi.yml
- filename: textforagents-com-legal-api-openapi.yml
  format: yaml
  label: textforagents-com Legal API
  slug: textforagents-com-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-legal-api-openapi.yml
- filename: textforagents-com-messages-api-openapi.yml
  format: yaml
  label: textforagents-com Messages API
  slug: textforagents-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-messages-api-openapi.yml
- filename: textforagents-com-support-api-openapi.yml
  format: yaml
  label: textforagents-com Support API
  slug: textforagents-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-support-api-openapi.yml
- filename: textforagents-com-wallet-creation-api-openapi.yml
  format: yaml
  label: textforagents-com Wallet Creation API
  slug: textforagents-com-wallet-creation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-wallet-creation-api-openapi.yml
- filename: textforagents-com-webhooks-api-openapi.yml
  format: yaml
  label: textforagents-com Webhooks API
  slug: textforagents-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-webhooks-api-openapi.yml
- filename: textforagents-com-x402-api-openapi.yml
  format: yaml
  label: textforagents-com X402 API
  slug: textforagents-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/textforagents-com/openapi/textforagents-com-x402-api-openapi.yml
auth_types: []
description: Authentication methods as described on TextForAgents product pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Textforagents Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: TextForAgents declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: TextForAgents
provider_slug: textforagents-com
scheme_count: 3
schemes:
- evidence: POST /register {account_name, payer_wallet} -> per-customer token (shown once, SHA-256 at rest).
  header: Authorization
  how_to_obtain: Returned by POST /register
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'POST /register {"operator": "your-name"} -> token (shown once); POST /trial with the Bearer token claims the one-time free grant.'
  header: Authorization
  how_to_obtain: Returned by POST /register
  location: header
  name: Bearer token
  type: http-bearer
- evidence: POST /adapters/gcp fetches your OAuth client lists with YOUR OWN Google access token (sent in the X-Provider-Token header, read-only, never stored or logged);
  header: X-Provider-Token
  how_to_obtain: Your own Google access token
  location: header
  name: X-Provider-Token
  type: apiKey
slug: textforagents-com-authentication
source_filename: textforagents-com-authentication.yml
source_heading: Authentication Profile
source_url: https://textforagents.com/products/mcp-oauth-client-interop-conformance/
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://textforagents.com/products/mcp-oauth-client-interop-conformance/\nsources:\n- https://textforagents.com/products/mcp-oauth-client-interop-conformance/\n- https://textforagents.com/products/mcp-oauth-remediation-verification/\n- https://textforagents.com/products/provider-mandate-census-agent-credentials/\n- https://textforagents.com/products/first-call-latency-witness/\ndescription: Authentication methods as described on TextForAgents product pages.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: POST /register {account_name, payer_wallet} -> per-customer token (shown once, SHA-256 at rest).\n  location: header\n  header: Authorization\n  how_to_obtain: Returned by POST /register\n- type: http-bearer\n  name: Bearer token\n  evidence: 'POST /register {\"operator\": \"your-name\"} -> token (shown once); POST /trial with the Bearer token claims the one-time\
  \ free grant.'\n  location: header\n  header: Authorization\n  how_to_obtain: Returned by POST /register\n- type: apiKey\n  name: X-Provider-Token\n  evidence: POST /adapters/gcp fetches your OAuth client lists with YOUR OWN Google access token (sent in the X-Provider-Token header, read-only,\n    never stored or logged);\n  location: header\n  header: X-Provider-Token\n  how_to_obtain: Your own Google access token\ndocs: https://textforagents.com/products/mcp-oauth-client-interop-conformance/\n"
source_yaml_url: https://artifacts.apis.io/textforagents-com/authentication/textforagents-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI
- Telephony
- SMS
- Agents
- API
---
