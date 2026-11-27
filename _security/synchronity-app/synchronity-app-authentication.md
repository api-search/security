---
anonymous_access: false
api_key_in: []
api_specs:
- filename: synchronity-app-auth-api-openapi.yml
  format: yaml
  label: Synchronity Auth API
  slug: synchronity-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-auth-api-openapi.yml
- filename: synchronity-app-cart-api-openapi.yml
  format: yaml
  label: Synchronity Cart API
  slug: synchronity-app-cart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-cart-api-openapi.yml
- filename: synchronity-app-checkout-api-openapi.yml
  format: yaml
  label: Synchronity Checkout API
  slug: synchronity-app-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-checkout-api-openapi.yml
- filename: synchronity-app-discovery-api-openapi.yml
  format: yaml
  label: Synchronity Discovery API
  slug: synchronity-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-discovery-api-openapi.yml
- filename: synchronity-app-multi-site-api-openapi.yml
  format: yaml
  label: Synchronity Multi Site API
  slug: synchronity-app-multi-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-multi-site-api-openapi.yml
- filename: synchronity-app-payments-api-openapi.yml
  format: yaml
  label: Synchronity Payments API
  slug: synchronity-app-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-payments-api-openapi.yml
- filename: synchronity-app-products-api-openapi.yml
  format: yaml
  label: Synchronity Products API
  slug: synchronity-app-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synchronity-app/openapi/synchronity-app-products-api-openapi.yml
auth_types: []
description: Authentication schemes for Synchronity
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Synchronity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synchronity declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Synchronity
provider_slug: synchronity-app
scheme_count: 1
schemes:
- evidence: 'The token goes into your MCP client''s Authorization: Bearer <token> header (the SDK handles this automatically).'
  header: Authorization
  how_to_obtain: POST https://api.synchronity.app/v1/auth/agents/register
  location: header
  name: Agent Identity Token
  type: http-bearer
slug: synchronity-app-authentication
source_filename: synchronity-app-authentication.yml
source_heading: Authentication Profile
source_url: https://synchronity.app/docs/concepts/identity
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://synchronity.app/docs/concepts/identity\nsources:\n- https://synchronity.app/docs/concepts/identity\n- https://synchronity.app/docs/quickstart\ndescription: Authentication schemes for Synchronity\nschemes:\n- type: http-bearer\n  name: Agent Identity Token\n  evidence: 'The token goes into your MCP client''s Authorization: Bearer <token> header (the SDK handles this automatically).'\n  location: header\n  header: Authorization\n  how_to_obtain: POST https://api.synchronity.app/v1/auth/agents/register\ndocs: https://synchronity.app/docs/concepts/identity\n"
source_yaml_url: https://artifacts.apis.io/synchronity-app/authentication/synchronity-app-authentication.yml
summary_line: 1 scheme
tags:
- Commerce
- AI
- Agents
- Integration
- E-commerce
---
