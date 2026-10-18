---
anonymous_access: false
api_key_in: []
api_specs:
- filename: karada-admin-api-openapi.yml
  format: yaml
  label: Karada AI Admin API
  slug: karada-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-admin-api-openapi.yml
- filename: karada-auth-api-openapi.yml
  format: yaml
  label: Karada AI Auth API
  slug: karada-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-auth-api-openapi.yml
- filename: karada-billing-api-openapi.yml
  format: yaml
  label: Karada AI Billing API
  slug: karada-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-billing-api-openapi.yml
- filename: karada-deployments-api-openapi.yml
  format: yaml
  label: Karada AI Deployments API
  slug: karada-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-deployments-api-openapi.yml
- filename: karada-feedback-api-openapi.yml
  format: yaml
  label: Karada AI Feedback API
  slug: karada-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-feedback-api-openapi.yml
- filename: karada-gateway-api-openapi.yml
  format: yaml
  label: Karada AI Gateway API
  slug: karada-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-gateway-api-openapi.yml
- filename: karada-marketplace-api-openapi.yml
  format: yaml
  label: Karada AI Marketplace API
  slug: karada-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-marketplace-api-openapi.yml
- filename: karada-mcp-api-openapi.yml
  format: yaml
  label: Karada AI MCP API
  slug: karada-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-mcp-api-openapi.yml
- filename: karada-newsletter-api-openapi.yml
  format: yaml
  label: Karada AI Newsletter API
  slug: karada-newsletter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-newsletter-api-openapi.yml
- filename: karada-pricing-api-openapi.yml
  format: yaml
  label: Karada AI Pricing API
  slug: karada-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-pricing-api-openapi.yml
- filename: karada-projects-api-openapi.yml
  format: yaml
  label: Karada AI Projects API
  slug: karada-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-projects-api-openapi.yml
- filename: karada-registry-api-openapi.yml
  format: yaml
  label: Karada AI Registry API
  slug: karada-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-registry-api-openapi.yml
- filename: karada-system-api-openapi.yml
  format: yaml
  label: Karada AI System API
  slug: karada-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-system-api-openapi.yml
- filename: karada-teams-api-openapi.yml
  format: yaml
  label: Karada AI Teams API
  slug: karada-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-teams-api-openapi.yml
- filename: karada-user-api-openapi.yml
  format: yaml
  label: Karada AI User API
  slug: karada-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/openapi/karada-user-api-openapi.yml
auth_types: []
description: Authentication methods published for Karada AI
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Karada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Karada AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Karada AI
provider_slug: karada
scheme_count: 2
schemes:
- authorize_url: https://api.karada.ai/api/v1/oauth/authorize
  evidence: Karada provides an end-to-end Managed OAuth 2.1 Provider & JWKS Identity Relay Engine.
  flows:
  - authorization_code
  how_to_obtain: User authenticates via a browser popup; the provider returns an authorization code which is exchanged for an RS256 JWT access token at the token endpoint.
  name: Karada Managed OAuth 2.1
  type: oauth2
- evidence: 'The MCP server sends requests with `Authorization: Bearer <token>`.'
  header: Authorization
  how_to_obtain: Access token is obtained from the Karada OAuth 2.1 token endpoint after completing the authorization_code flow.
  location: header
  name: Bearer JWT
  type: http-bearer
slug: karada-authentication
source_filename: karada-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.karada.ai/guides/oauth-backend-auth.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.karada.ai/guides/oauth-backend-auth.md\nsources:\n- https://docs.karada.ai/guides/oauth-backend-auth.md\n- https://docs.karada.ai/quickstart.md\ndescription: Authentication methods published for Karada AI\nschemes:\n- type: oauth2\n  name: Karada Managed OAuth 2.1\n  evidence: Karada provides an end-to-end Managed OAuth 2.1 Provider & JWKS Identity Relay Engine.\n  flows:\n  - authorization_code\n  authorize_url: https://api.karada.ai/api/v1/oauth/authorize\n  how_to_obtain: User authenticates via a browser popup; the provider returns an authorization code which is exchanged for an RS256 JWT access\n    token at the token endpoint.\n- type: http-bearer\n  name: Bearer JWT\n  evidence: 'The MCP server sends requests with `Authorization: Bearer <token>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Access token is obtained from the Karada OAuth 2.1\
  \ token endpoint after completing the authorization_code flow.\ndocs: https://docs.karada.ai/guides/oauth-backend-auth.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karada/refs/heads/main/authentication/karada-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Platform
- MCP
- Automation
---
