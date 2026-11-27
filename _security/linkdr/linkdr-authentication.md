---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkdr-admin-mcp-api-openapi.yml
  format: yaml
  label: LinkDR MCP Admin MCP API
  slug: linkdr-admin-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-admin-mcp-api-openapi.yml
- filename: linkdr-agent-resources-api-openapi.yml
  format: yaml
  label: LinkDR MCP Agent resources API
  slug: linkdr-agent-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-agent-resources-api-openapi.yml
- filename: linkdr-mcp-api-openapi.yml
  format: yaml
  label: LinkDR MCP MCP API
  slug: linkdr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-mcp-api-openapi.yml
- filename: linkdr-public-data-api-openapi.yml
  format: yaml
  label: LinkDR MCP Public data API
  slug: linkdr-public-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-public-data-api-openapi.yml
- filename: linkdr-system-api-openapi.yml
  format: yaml
  label: LinkDR MCP System API
  slug: linkdr-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-system-api-openapi.yml
auth_types: []
description: LinkDR MCP uses OAuth 2.0 with PKCE for admin authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LinkDR MCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkDR MCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LinkDR MCP
provider_slug: linkdr
scheme_count: 1
schemes:
- authorize_url: https://linkdr.com/.well-known/oauth-protected-resource/mcp/admin
  evidence: The client starts OAuth (PKCE). A browser opens to LinkDR login if you are not already signed in.
  flows:
  - authorization_code
  how_to_obtain: User signs in via browser; consent page grants access and returns an access token.
  name: LinkDR OAuth
  type: oauth2
slug: linkdr-authentication
source_filename: linkdr-authentication.yml
source_heading: Authentication Profile
source_url: https://linkdr.com/docs/admin/auth
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://linkdr.com/docs/admin/auth\nsources:\n- https://linkdr.com/docs/admin/auth\ndescription: LinkDR MCP uses OAuth 2.0 with PKCE for admin authentication.\nschemes:\n- type: oauth2\n  name: LinkDR OAuth\n  evidence: The client starts OAuth (PKCE). A browser opens to LinkDR login if you are not already signed in.\n  flows:\n  - authorization_code\n  authorize_url: https://linkdr.com/.well-known/oauth-protected-resource/mcp/admin\n  how_to_obtain: User signs in via browser; consent page grants access and returns an access token.\ndocs: https://linkdr.com/docs/admin/auth\n"
source_yaml_url: https://artifacts.apis.io/linkdr/authentication/linkdr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SEO
- Backlink
- Artificial Intelligence
- Software-as-a-Service
---
