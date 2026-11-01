---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shipstar-ai-authentication-api-openapi.yml
  format: yaml
  label: shipstar-ai Authentication API
  slug: shipstar-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-authentication-api-openapi.yml
- filename: shipstar-ai-banner-api-openapi.yml
  format: yaml
  label: shipstar-ai Banner API
  slug: shipstar-ai-banner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-banner-api-openapi.yml
- filename: shipstar-ai-blog-api-openapi.yml
  format: yaml
  label: shipstar-ai Blog API
  slug: shipstar-ai-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-blog-api-openapi.yml
- filename: shipstar-ai-changelog-api-openapi.yml
  format: yaml
  label: shipstar-ai Changelog API
  slug: shipstar-ai-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-changelog-api-openapi.yml
- filename: shipstar-ai-changelog-subscriptions-api-openapi.yml
  format: yaml
  label: shipstar-ai Changelog Subscriptions API
  slug: shipstar-ai-changelog-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-changelog-subscriptions-api-openapi.yml
- filename: shipstar-ai-health-api-openapi.yml
  format: yaml
  label: shipstar-ai Health API
  slug: shipstar-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-health-api-openapi.yml
- filename: shipstar-ai-kb-api-openapi.yml
  format: yaml
  label: shipstar-ai Kb API
  slug: shipstar-ai-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-kb-api-openapi.yml
- filename: shipstar-ai-mailing-lists-api-openapi.yml
  format: yaml
  label: shipstar-ai Mailing Lists API
  slug: shipstar-ai-mailing-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-mailing-lists-api-openapi.yml
- filename: shipstar-ai-team-invitations-api-openapi.yml
  format: yaml
  label: shipstar-ai Team Invitations API
  slug: shipstar-ai-team-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-team-invitations-api-openapi.yml
auth_types: []
description: Authentication schemes for Shipstar API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Shipstar Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: shipstar-ai declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: shipstar-ai
provider_slug: shipstar-ai
scheme_count: 3
schemes:
- evidence: 'API keys are used for programmatic access to the Shipstar API. Include your key in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Create in the Dashboard
  location: header
  name: API Key
  type: http-bearer
- evidence: 'Use the JWT token the same way as an API key:'
  header: Authorization
  how_to_obtain: Login via `/api/internal/auth/jwt/login`
  location: header
  name: JWT Session Token
  type: http-bearer
- authorize_url: https://api.shipstar.ai/oauth/authorize
  evidence: Shipstar's backend is a full OAuth 2.1 authorization server.
  how_to_obtain: Dynamic client registration via `POST /oauth/register`
  name: Shipstar MCP OAuth
  scopes:
  - mcp
  token_url: https://api.shipstar.ai/oauth/token
  type: oauth2
slug: shipstar-ai-authentication
source_filename: shipstar-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.shipstar.ai/guides/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.shipstar.ai/guides/authentication.md\nsources:\n- https://docs.shipstar.ai/guides/authentication.md\n- https://docs.shipstar.ai/mcp/oauth.md\n- https://docs.shipstar.ai/api-reference/authentication.md\n- https://docs.shipstar.ai/quickstart.md\ndescription: Authentication schemes for Shipstar API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'API keys are used for programmatic access to the Shipstar API. Include your key in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create in the Dashboard\n- type: http-bearer\n  name: JWT Session Token\n  evidence: 'Use the JWT token the same way as an API key:'\n  location: header\n  header: Authorization\n  how_to_obtain: Login via `/api/internal/auth/jwt/login`\n- type: oauth2\n  name: Shipstar MCP OAuth\n  evidence: Shipstar's backend is a full OAuth 2.1 authorization\
  \ server.\n  token_url: https://api.shipstar.ai/oauth/token\n  authorize_url: https://api.shipstar.ai/oauth/authorize\n  scopes:\n  - mcp\n  how_to_obtain: Dynamic client registration via `POST /oauth/register`\ndocs: https://docs.shipstar.ai/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/shipstar-ai/authentication/shipstar-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Marketing
- DeveloperTools
- Automation
- OpenSource
---
