---
anonymous_access: false
api_key_in: []
api_specs:
- filename: useagentbank-payouts-api-openapi.yml
  format: yaml
  label: AgentBank Payouts API
  slug: useagentbank-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/useagentbank/openapi/useagentbank-payouts-api-openapi.yml
auth_types: []
description: Authentication methods for AgentBank APIs as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Useagentbank Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentBank declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentBank
provider_slug: useagentbank
scheme_count: 1
schemes:
- evidence: Ed25519 request signing for the Partner API and JWT login for the portal API.
  header: x-agentbank-signature
  how_to_obtain: Obtain a merchant Ed25519 key pair during onboarding; the partner ID (`mp_...`) is returned during onboarding and the private key is used to sign each request as described.
  location: header
  name: Ed25519 request signing
  type: other
slug: useagentbank-authentication
source_filename: useagentbank-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.useagentbank.com/getting-started/hosted-oauth.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.useagentbank.com/getting-started/hosted-oauth.md\nsources:\n- https://docs.useagentbank.com/getting-started/hosted-oauth.md\n- https://docs.useagentbank.com/getting-started/authentication.md\n- https://docs.useagentbank.com/partner-api/authentication.md\n- https://docs.useagentbank.com/reference/tools/get-token-allowance.md\ndescription: Authentication methods for AgentBank APIs as documented.\nschemes:\n- type: other\n  name: Ed25519 request signing\n  evidence: Ed25519 request signing for the Partner API and JWT login for the portal API.\n  location: header\n  header: x-agentbank-signature\n  how_to_obtain: Obtain a merchant Ed25519 key pair during onboarding; the partner ID (`mp_...`) is returned during onboarding and the private\n    key is used to sign each request as described.\nnote: No OAuth flow URLs or scopes are provided in the documentation pages. 1 extracted\
  \ row(s) were dropped because their quote was not on the\n  page.\ndocs: https://docs.useagentbank.com/getting-started/hosted-oauth.md\n"
source_yaml_url: https://artifacts.apis.io/useagentbank/authentication/useagentbank-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- AI
- Banking
- Crypto
- Payments
---
