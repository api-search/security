---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: createprints-ai-account-api-openapi.yml
  format: yaml
  label: Create Prints Account API
  slug: createprints-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-account-api-openapi.yml
- filename: createprints-ai-artwork-api-openapi.yml
  format: yaml
  label: Create Prints Artwork API
  slug: createprints-ai-artwork-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-artwork-api-openapi.yml
- filename: createprints-ai-checkout-api-openapi.yml
  format: yaml
  label: Create Prints Checkout API
  slug: createprints-ai-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-checkout-api-openapi.yml
- filename: createprints-ai-orders-api-openapi.yml
  format: yaml
  label: Create Prints Orders API
  slug: createprints-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-orders-api-openapi.yml
- filename: createprints-ai-product-discovery-api-openapi.yml
  format: yaml
  label: Create Prints Product discovery API
  slug: createprints-ai-product-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-product-discovery-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Create Prints Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Create Prints secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Create Prints
provider_slug: createprints-ai
scheme_count: 3
schemes:
- description: Create Prints account API key beginning with `cp_`. Required scopes vary by operation.
  in: header
  name: agentApiKey
  parameter: X-API-Key
  sources:
  - openapi/createprints-ai-openapi.yml
  type: apiKey
- description: Account API key (`cp_…`) or MCP OAuth token (`cp_mcp_access_…`) in Authorization.
  name: agentBearer
  scheme: bearer
  sources:
  - openapi/createprints-ai-openapi.yml
  type: http
- description: Create Prints OAuth 2.0 authorization-code flow with PKCE for MCP and agent clients.
  flows:
  - authorizationUrl: https://api.createprints.ai/api/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.createprints.ai/api/oauth/token
  name: oauth2
  sources:
  - openapi/createprints-ai-openapi.yml
  type: oauth2
slug: createprints-ai-authentication
source_filename: createprints-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.createprints.ai/auth.md\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: agentApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Create Prints account API key beginning with `cp_`. Required scopes vary by operation.\n  sources:\n  - openapi/createprints-ai-openapi.yml\n- name: agentBearer\n  type: http\n  scheme: bearer\n  description: Account API key (`cp_…`) or MCP OAuth token (`cp_mcp_access_…`) in Authorization.\n  sources:\n  - openapi/createprints-ai-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.createprints.ai/api/oauth/authorize\n    tokenUrl: https://api.createprints.ai/api/oauth/token\n    scopes: 6\n  description: Create Prints OAuth 2.0 authorization-code flow with PKCE for MCP and agent clients.\n  sources:\n  - openapi/createprints-ai-openapi.yml\n\
  docs: https://www.createprints.ai/auth.md\noauth2_details:\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  pkce: S256 only\n  token_endpoint_auth_methods_supported:\n  - none\n  client_registration: OAuth 2.0 Dynamic Client Registration (RFC 7591) at https://api.createprints.ai/api/oauth/register;\n    no manual sign-up or API key required\n  authorization_server_metadata: 'https://api.createprints.ai/.well-known/oauth-authorization-server (RFC 8414;\n    includes an agent_auth block declaring identity_types_supported: [\"service_auth\"])'\n  protected_resource_metadata: https://mcp.createprints.ai/.well-known/oauth-protected-resource/mcp (RFC 9728),\n    advertised via WWW-Authenticate on a 401 from the MCP endpoint\n  revocation_endpoint: https://api.createprints.ai/api/mcp/revoke\n  resource_indicator: resource parameter sent on the authorize request\napi_keys:\n  prefix: cp_\n  oauth_token_prefix: cp_mcp_access_\n  issued_from: self-service agent API key from\
  \ the signed-in account page (per the developers page)\n  headers:\n  - X-API-Key\n  - 'Authorization: Bearer'\nnote: Docs-read only; no auth, token, registration or revocation endpoint was called.\ndocs_also:\n- https://www.createprints.ai/developers\n"
source_yaml_url: https://artifacts.apis.io/createprints-ai/authentication/createprints-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- AI Art
- Generative AI
- Art Prints
- Print on Demand
- E-Commerce
- Interior Design
- MCP
---
