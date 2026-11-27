---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deskcrew-io-app-api-openapi.yml
  format: yaml
  label: DeskCrew App API
  slug: deskcrew-io-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-app-api-openapi.yml
- filename: deskcrew-io-billing-api-openapi.yml
  format: yaml
  label: DeskCrew Billing API
  slug: deskcrew-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-billing-api-openapi.yml
- filename: deskcrew-io-bounties-api-openapi.yml
  format: yaml
  label: DeskCrew Bounties API
  slug: deskcrew-io-bounties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-bounties-api-openapi.yml
- filename: deskcrew-io-changelog-api-openapi.yml
  format: yaml
  label: DeskCrew Changelog API
  slug: deskcrew-io-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-changelog-api-openapi.yml
- filename: deskcrew-io-changes-api-openapi.yml
  format: yaml
  label: DeskCrew Changes API
  slug: deskcrew-io-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-changes-api-openapi.yml
- filename: deskcrew-io-customers-api-openapi.yml
  format: yaml
  label: DeskCrew Customers API
  slug: deskcrew-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-customers-api-openapi.yml
- filename: deskcrew-io-devices-api-openapi.yml
  format: yaml
  label: DeskCrew Devices API
  slug: deskcrew-io-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-devices-api-openapi.yml
- filename: deskcrew-io-errors-api-openapi.yml
  format: yaml
  label: DeskCrew Errors API
  slug: deskcrew-io-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-errors-api-openapi.yml
- filename: deskcrew-io-issues-api-openapi.yml
  format: yaml
  label: DeskCrew Issues API
  slug: deskcrew-io-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-issues-api-openapi.yml
- filename: deskcrew-io-kb-api-openapi.yml
  format: yaml
  label: DeskCrew Kb API
  slug: deskcrew-io-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-kb-api-openapi.yml
- filename: deskcrew-io-me-api-openapi.yml
  format: yaml
  label: DeskCrew Me API
  slug: deskcrew-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-me-api-openapi.yml
- filename: deskcrew-io-paid-agent-tools-api-openapi.yml
  format: yaml
  label: DeskCrew Paid agent tools API
  slug: deskcrew-io-paid-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-paid-agent-tools-api-openapi.yml
- filename: deskcrew-io-tickets-api-openapi.yml
  format: yaml
  label: DeskCrew Tickets API
  slug: deskcrew-io-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-tickets-api-openapi.yml
- filename: deskcrew-io-webhooks-api-openapi.yml
  format: yaml
  label: DeskCrew Webhooks API
  slug: deskcrew-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-webhooks-api-openapi.yml
auth_types: []
description: 'DeskCrew supports two authentication mechanisms: a bearer token for credentialed agents and a custom payment‑signature flow for anonymous agents using the x402 protocol.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DeskCrew Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeskCrew declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DeskCrew
provider_slug: deskcrew-io
scheme_count: 2
schemes:
- evidence: 'Send it as Authorization: Bearer mcp_…'
  header: Authorization
  how_to_obtain: Create a free DeskCrew account, go to Dashboard → Agents → mint a credential; the credential begins with "mcp_" and is used as a bearer token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Sign a USDC transferWithAuthorization for the quoted terms and repeat the call with the base64 payload in the X-PAYMENT header.
  header: X-PAYMENT
  how_to_obtain: Generate a wallet, sign an EIP‑3009 USDC TransferWithAuthorization for the quoted payment terms, base64‑encode the payload, and include it in the X-PAYMENT header.
  location: header
  name: x402 payment signature
  type: other
slug: deskcrew-io-authentication
source_filename: deskcrew-io-authentication.yml
source_heading: Authentication Profile
source_url: https://deskcrew.io/agents
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://deskcrew.io/agents\nsources:\n- https://deskcrew.io/agents\ndescription: 'DeskCrew supports two authentication mechanisms: a bearer token for credentialed agents and a custom payment‑signature flow for\n  anonymous agents using the x402 protocol.'\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send it as Authorization: Bearer mcp_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a free DeskCrew account, go to Dashboard → Agents → mint a credential; the credential begins with \"mcp_\" and is used as\n    a bearer token.\n- type: other\n  name: x402 payment signature\n  evidence: Sign a USDC transferWithAuthorization for the quoted terms and repeat the call with the base64 payload in the X-PAYMENT header.\n  location: header\n  header: X-PAYMENT\n  how_to_obtain: Generate a wallet, sign an EIP‑3009 USDC TransferWithAuthorization for\
  \ the quoted payment terms, base64‑encode the payload, and\n    include it in the X-PAYMENT header.\ndocs: https://deskcrew.io/agents\n"
source_yaml_url: https://artifacts.apis.io/deskcrew-io/authentication/deskcrew-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Help Desk
- AI Agents
- MCP
- Support
---
