---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nevermined-app-agent-services-catalog-api-openapi.yml
  format: yaml
  label: Nevermined Agent Services Catalog API
  slug: nevermined-app-agent-services-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-agent-services-catalog-api-openapi.yml
- filename: nevermined-app-ard-registry-api-openapi.yml
  format: yaml
  label: Nevermined ARD Registry API
  slug: nevermined-app-ard-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-ard-registry-api-openapi.yml
- filename: nevermined-app-delegation-api-openapi.yml
  format: yaml
  label: Nevermined Delegation API
  slug: nevermined-app-delegation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-delegation-api-openapi.yml
- filename: nevermined-app-info-api-openapi.yml
  format: yaml
  label: Nevermined Info API
  slug: nevermined-app-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-info-api-openapi.yml
- filename: nevermined-app-oauth-api-openapi.yml
  format: yaml
  label: Nevermined OAuth API
  slug: nevermined-app-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-oauth-api-openapi.yml
- filename: nevermined-app-organizations-integration-api-openapi.yml
  format: yaml
  label: Nevermined Organizations - Integration API
  slug: nevermined-app-organizations-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-organizations-integration-api-openapi.yml
- filename: nevermined-app-payment-methods-api-openapi.yml
  format: yaml
  label: Nevermined Payment Methods API
  slug: nevermined-app-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-payment-methods-api-openapi.yml
- filename: nevermined-app-protocol-api-openapi.yml
  format: yaml
  label: Nevermined Protocol API
  slug: nevermined-app-protocol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-protocol-api-openapi.yml
- filename: nevermined-app-router-api-openapi.yml
  format: yaml
  label: Nevermined Router API
  slug: nevermined-app-router-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-router-api-openapi.yml
- filename: nevermined-app-subscription-agent-api-openapi.yml
  format: yaml
  label: Nevermined Subscription - Agent API
  slug: nevermined-app-subscription-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-subscription-agent-api-openapi.yml
- filename: nevermined-app-subscription-api-openapi.yml
  format: yaml
  label: Nevermined Subscription API
  slug: nevermined-app-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-subscription-api-openapi.yml
- filename: nevermined-app-well-known-api-openapi.yml
  format: yaml
  label: Nevermined Well Known API
  slug: nevermined-app-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-well-known-api-openapi.yml
- filename: nevermined-app-x402-api-openapi.yml
  format: yaml
  label: Nevermined X402 API
  slug: nevermined-app-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nevermined-app/openapi/nevermined-app-x402-api-openapi.yml
auth_types: []
description: Authentication schemes for Nevermined API as described in the provided documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Nevermined Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nevermined declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Nevermined
provider_slug: nevermined-app
scheme_count: 3
schemes:
- evidence: Use it as a Bearer token on REST calls
  header: Authorization
  how_to_obtain: Obtain a Nevermined API key via the embedded login flow, manual paste, device flow, or OAuth as described in the Get a Nevermined API Key guide.
  location: header
  name: Nevermined API Key
  type: http-bearer
- evidence: A headless agent with no browser and no localhost can still get a key with a human’s approval through the device flow (RFC 8628).
  how_to_obtain: Use the RFC 8628 device flow as described in the Authentication overview page.
  name: Device Flow
  type: oauth2
- evidence: Authorization Code + PKCE Browser-based MCP clients paying for a specific agent — and AI assistants obtaining a commerce grant.
  how_to_obtain: Use the Authorization Code with PKCE flow as described in the Authentication overview page.
  name: Authorization Code + PKCE
  type: oauth2
slug: nevermined-app-authentication
source_filename: nevermined-app-authentication.yml
source_heading: Authentication Profile
source_url: https://nevermined.ai/docs/agents-guide/get-api-key.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nevermined.ai/docs/agents-guide/get-api-key.md\nsources:\n- https://nevermined.ai/docs/agents-guide/get-api-key.md\n- https://nevermined.ai/docs/integrate/authentication/overview\n- https://nevermined.ai/docs/agents-guide/get-api-key\n- https://nevermined.ai/docs/api-reference/protocol/get-access-token\ndescription: Authentication schemes for Nevermined API as described in the provided documentation pages.\nschemes:\n- type: http-bearer\n  name: Nevermined API Key\n  evidence: Use it as a Bearer token on REST calls\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a Nevermined API key via the embedded login flow, manual paste, device flow, or OAuth as described in the Get a Nevermined\n    API Key guide.\n- type: oauth2\n  name: Device Flow\n  evidence: A headless agent with no browser and no localhost can still get a key with a human’s approval through\
  \ the device flow (RFC 8628).\n  how_to_obtain: Use the RFC 8628 device flow as described in the Authentication overview page.\n- type: oauth2\n  name: Authorization Code + PKCE\n  evidence: Authorization Code + PKCE Browser-based MCP clients paying for a specific agent — and AI assistants obtaining a commerce grant.\n  how_to_obtain: Use the Authorization Code with PKCE flow as described in the Authentication overview page.\ndocs: https://nevermined.ai/docs/agents-guide/get-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/nevermined-app/authentication/nevermined-app-authentication.yml
summary_line: 3 schemes
tags:
- Payments
- Artificial Intelligence
- Platform
- Fintech
- AI Agents
---
