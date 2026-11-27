---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apier-no-account-api-openapi.yml
  format: yaml
  label: Apier.no Account API
  slug: apier-no-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-account-api-openapi.yml
- filename: apier-no-actions-api-openapi.yml
  format: yaml
  label: Apier.no Actions API
  slug: apier-no-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-actions-api-openapi.yml
- filename: apier-no-admin-api-openapi.yml
  format: yaml
  label: Apier.no Admin API
  slug: apier-no-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-admin-api-openapi.yml
- filename: apier-no-altinn-api-openapi.yml
  format: yaml
  label: Apier.no Altinn API
  slug: apier-no-altinn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-altinn-api-openapi.yml
- filename: apier-no-auth-gateway-api-openapi.yml
  format: yaml
  label: Apier.no Auth Gateway API
  slug: apier-no-auth-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-auth-gateway-api-openapi.yml
- filename: apier-no-brreg-api-openapi.yml
  format: yaml
  label: Apier.no Brreg API
  slug: apier-no-brreg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-brreg-api-openapi.yml
- filename: apier-no-changes-api-openapi.yml
  format: yaml
  label: Apier.no Changes API
  slug: apier-no-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-changes-api-openapi.yml
- filename: apier-no-company-api-openapi.yml
  format: yaml
  label: Apier.no Company API
  slug: apier-no-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-company-api-openapi.yml
- filename: apier-no-discovery-api-openapi.yml
  format: yaml
  label: Apier.no Discovery API
  slug: apier-no-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-discovery-api-openapi.yml
- filename: apier-no-fullmakt-api-openapi.yml
  format: yaml
  label: Apier.no Fullmakt API
  slug: apier-no-fullmakt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-fullmakt-api-openapi.yml
- filename: apier-no-infrastructure-api-openapi.yml
  format: yaml
  label: Apier.no Infrastructure API
  slug: apier-no-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-infrastructure-api-openapi.yml
- filename: apier-no-knowledge-api-openapi.yml
  format: yaml
  label: Apier.no Knowledge API
  slug: apier-no-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-knowledge-api-openapi.yml
- filename: apier-no-privacy-api-openapi.yml
  format: yaml
  label: Apier.no Privacy API
  slug: apier-no-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-privacy-api-openapi.yml
- filename: apier-no-public-api-openapi.yml
  format: yaml
  label: Apier.no Public API
  slug: apier-no-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-public-api-openapi.yml
- filename: apier-no-sandbox-api-openapi.yml
  format: yaml
  label: Apier.no Sandbox API
  slug: apier-no-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-sandbox-api-openapi.yml
- filename: apier-no-subscriptions-api-openapi.yml
  format: yaml
  label: Apier.no Subscriptions API
  slug: apier-no-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Apier.no Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apier.no declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Apier.no
provider_slug: apier-no
scheme_count: 5
schemes:
- description: 'API key issued by Apier. Include as: Authorization: Bearer <your-key>.'
  name: BearerAuth
  scheme: bearer
  type: http
- description: 'Frictionless sandbox bearer. Format: Authorization: Bearer apier_sandbox_test_<suffix>.'
  name: SandboxBearerAuth
  scheme: bearer
  type: http
- description: Admin API key (ADMIN_API_KEY env var).
  name: AdminBearerAuth
  scheme: bearer
  type: http
- description: Supabase Auth session cookie set by the /confirm interstitial's POST to /api/auth/verify after a magic-link sign-in.
  in: cookie
  name: SessionCookieAuth
  type: apiKey
- description: OAuth 2.1 sign-in for the remote MCP endpoint (/api/mcp).
  name: McpOAuth
  type: oauth2
slug: apier-no-authentication
source_filename: apier-no-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://www.apier.no/docs/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    name: BearerAuth\n    description: \"API key issued by Apier. Include as: Authorization: Bearer <your-key>.\"\n  - type: http\n    scheme: bearer\n    name: SandboxBearerAuth\n    description: \"Frictionless sandbox bearer. Format: Authorization: Bearer apier_sandbox_test_<suffix>.\"\n  - type: http\n    scheme: bearer\n    name: AdminBearerAuth\n    description: \"Admin API key (ADMIN_API_KEY env var).\"\n  - type: apiKey\n    in: cookie\n    name: SessionCookieAuth\n    description: \"Supabase Auth session cookie set by the /confirm interstitial's POST to /api/auth/verify after a magic-link sign-in.\"\n  - type: oauth2\n    name: McpOAuth\n    description: \"OAuth 2.1 sign-in for the remote MCP endpoint (/api/mcp).\"\n"
source_yaml_url: https://artifacts.apis.io/apier-no/authentication/apier-no-authentication.yml
summary_line: 5 schemes
tags:
- Norwegian
- Company Data
- MCP
- Verification
---
