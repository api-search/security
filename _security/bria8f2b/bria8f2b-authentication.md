---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bria8f2b-ai-search-api-openapi.yml
  format: yaml
  label: Bria8f2b AI Search API
  slug: bria8f2b-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-ai-search-api-openapi.yml
- filename: bria8f2b-campaign-generation-coming-soon-api-openapi.yml
  format: yaml
  label: Bria8f2b Campaign Generation (Coming soon) API
  slug: bria8f2b-campaign-generation-coming-soon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-campaign-generation-coming-soon-api-openapi.yml
- filename: bria8f2b-image-editing-api-openapi.yml
  format: yaml
  label: Bria8f2b Image Editing API
  slug: bria8f2b-image-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-image-editing-api-openapi.yml
- filename: bria8f2b-image-generation-api-openapi.yml
  format: yaml
  label: Bria8f2b Image Generation API
  slug: bria8f2b-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-image-generation-api-openapi.yml
- filename: bria8f2b-image-onboarding-api-openapi.yml
  format: yaml
  label: Bria8f2b Image Onboarding API
  slug: bria8f2b-image-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-image-onboarding-api-openapi.yml
- filename: bria8f2b-product-shots-generation-api-openapi.yml
  format: yaml
  label: Bria8f2b Product Shots Generation API
  slug: bria8f2b-product-shots-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-product-shots-generation-api-openapi.yml
- filename: bria8f2b-tailored-generation-api-openapi.yml
  format: yaml
  label: Bria8f2b Tailored Generation API
  slug: bria8f2b-tailored-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-tailored-generation-api-openapi.yml
- filename: bria8f2b-video-editing-api-openapi.yml
  format: yaml
  label: Bria8f2b Video Editing API
  slug: bria8f2b-video-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/openapi/bria8f2b-video-editing-api-openapi.yml
auth_types: []
description: Bria uses organization‑level API tokens and also supports OAuth 2.1 bearer tokens for the hosted MCP server.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bria8F2B Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bria8f2b declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bria8f2b
provider_slug: bria8f2b
scheme_count: 2
schemes:
- evidence: 'Pass the token in the `api_token` request header:'
  header: api_token
  how_to_obtain: Create a token in the Bria Console → Organization management → API keys.
  location: header
  name: api_token
  type: apiKey
- authorize_url: https://mcp.prod.bria-api.com/.well-known/oauth-authorization-server
  evidence: The hosted server implements the MCP authorization flow (OAuth 2.1 with PKCE, dynamic client registration and discovery at `https://mcp.prod.bria-api.com/.well-known/oauth-authorization-server`).
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Use the MCP OAuth flow; clients obtain a bearer token via the discovery endpoint and PKCE flow.
  location: header
  name: OAuth 2.1 bearer token
  type: oauth2
slug: bria8f2b-authentication
source_filename: bria8f2b-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bria.ai/getting-started/authentication.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bria.ai/getting-started/authentication.md\nsources:\n- https://docs.bria.ai/getting-started/authentication.md\n- https://docs.bria.ai/mcp-authentication.md\n- https://docs.bria.ai/getting-started/asset-retention.md\n- https://docs.bria.ai/getting-started/async-requests.md\ndescription: Bria uses organization‑level API tokens and also supports OAuth 2.1 bearer tokens for the hosted MCP server.\nschemes:\n- type: apiKey\n  name: api_token\n  evidence: 'Pass the token in the `api_token` request header:'\n  location: header\n  header: api_token\n  how_to_obtain: Create a token in the Bria Console → Organization management → API keys.\n- type: oauth2\n  name: OAuth 2.1 bearer token\n  evidence: The hosted server implements the MCP authorization flow (OAuth 2.1 with PKCE, dynamic client registration and discovery at `https://mcp.prod.bria-api.com/.well-known/oauth-authorization-server`).\n\
  \  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.prod.bria-api.com/.well-known/oauth-authorization-server\n  how_to_obtain: Use the MCP OAuth flow; clients obtain a bearer token via the discovery endpoint and PKCE flow.\ndocs: https://docs.bria.ai/getting-started/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bria8f2b/refs/heads/main/authentication/bria8f2b-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Visual
- Enterprise
- Imaging
---
