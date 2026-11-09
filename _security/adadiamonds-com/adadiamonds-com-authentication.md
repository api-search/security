---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adadiamonds-com-agentic-checkout-acp-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (ACP) API
  slug: adadiamonds-com-agentic-checkout-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-acp-api-openapi.yml
- filename: adadiamonds-com-agentic-checkout-hosted-link-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (hosted link) API
  slug: adadiamonds-com-agentic-checkout-hosted-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-hosted-link-api-openapi.yml
- filename: adadiamonds-com-agentic-checkout-ucp-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (UCP) API
  slug: adadiamonds-com-agentic-checkout-ucp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-ucp-api-openapi.yml
- filename: adadiamonds-com-agentic-commerce-discovery-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic commerce discovery API
  slug: adadiamonds-com-agentic-commerce-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-commerce-discovery-api-openapi.yml
- filename: adadiamonds-com-appointments-api-openapi.yml
  format: yaml
  label: Ada Diamonds Appointments API
  slug: adadiamonds-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-appointments-api-openapi.yml
- filename: adadiamonds-com-bulk-api-openapi.yml
  format: yaml
  label: Ada Diamonds Bulk API
  slug: adadiamonds-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-bulk-api-openapi.yml
- filename: adadiamonds-com-catalog-api-openapi.yml
  format: yaml
  label: Ada Diamonds Catalog API
  slug: adadiamonds-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-catalog-api-openapi.yml
- filename: adadiamonds-com-content-api-openapi.yml
  format: yaml
  label: Ada Diamonds Content API
  slug: adadiamonds-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-content-api-openapi.yml
- filename: adadiamonds-com-discovery-api-openapi.yml
  format: yaml
  label: Ada Diamonds Discovery API
  slug: adadiamonds-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-discovery-api-openapi.yml
- filename: adadiamonds-com-mcp-api-openapi.yml
  format: yaml
  label: Ada Diamonds MCP API
  slug: adadiamonds-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-mcp-api-openapi.yml
- filename: adadiamonds-com-onboarding-api-openapi.yml
  format: yaml
  label: Ada Diamonds Onboarding API
  slug: adadiamonds-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-onboarding-api-openapi.yml
- filename: adadiamonds-com-search-api-openapi.yml
  format: yaml
  label: Ada Diamonds Search API
  slug: adadiamonds-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-search-api-openapi.yml
auth_types: []
description: Authentication methods published by Ada Diamonds
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Adadiamonds Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ada Diamonds declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ada Diamonds
provider_slug: adadiamonds-com
scheme_count: 2
schemes:
- evidence: 'Send it as Authorization: Bearer <key> or X-Ada-Api-Key: <key> .'
  header: X-Ada-Api-Key
  how_to_obtain: POST https://www.adadiamonds.com/api/v1/keys
  location: header
  name: X-Ada-Api-Key
  type: apiKey
- authorize_url: https://www.adadiamonds.com/oauth/authorize
  evidence: Ada Diamonds runs an OAuth 2.1 authorization server at https://www.adadiamonds.com , with metadata at /.well-known/oauth-authorization-server .
  flows:
  - client_credentials
  - authorization_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:workos:agent-auth:grant-type:claim
  how_to_obtain: POST https://www.adadiamonds.com/api/oauth/token
  name: Ada Diamonds OAuth 2.1
  scopes:
  - catalog:read
  - content:read
  - profile:read
  - orders:read
  - cart:write
  - appointments:write
  type: oauth2
slug: adadiamonds-com-authentication
source_filename: adadiamonds-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.adadiamonds.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.adadiamonds.com/.well-known/oauth-authorization-server\nsources:\n- https://www.adadiamonds.com/.well-known/oauth-authorization-server\n- https://www.adadiamonds.com/auth.md\n- https://www.adadiamonds.com/developers/authentication\ndescription: Authentication methods published by Ada Diamonds\nschemes:\n- type: apiKey\n  name: X-Ada-Api-Key\n  evidence: 'Send it as Authorization: Bearer <key> or X-Ada-Api-Key: <key> .'\n  location: header\n  header: X-Ada-Api-Key\n  how_to_obtain: POST https://www.adadiamonds.com/api/v1/keys\n- type: oauth2\n  name: Ada Diamonds OAuth 2.1\n  evidence: Ada Diamonds runs an OAuth 2.1 authorization server at https://www.adadiamonds.com , with metadata at /.well-known/oauth-authorization-server\n    .\n  flows:\n  - client_credentials\n  - authorization_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:workos:agent-auth:grant-type:claim\n\
  \  authorize_url: https://www.adadiamonds.com/oauth/authorize\n  scopes:\n  - catalog:read\n  - content:read\n  - profile:read\n  - orders:read\n  - cart:write\n  - appointments:write\n  how_to_obtain: POST https://www.adadiamonds.com/api/oauth/token\ndocs: https://www.adadiamonds.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/adadiamonds-com/authentication/adadiamonds-com-authentication.yml
summary_line: 2 schemes
tags:
- Jewelry
- Lab Diamonds
- Engagement Rings
- New York
- E-Commerce
---
