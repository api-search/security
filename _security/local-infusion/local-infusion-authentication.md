---
api_key_in:
- header
api_specs:
- filename: local-infusion-wp-v2-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Content API
  slug: local-infusion-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-wp-v2-api-openapi.yml
- filename: local-infusion-mcp-api-openapi.yml
  format: yaml
  label: Local Infusion MCP API
  slug: local-infusion-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-mcp-api-openapi.yml
- filename: local-infusion-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Abilities API
  slug: local-infusion-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-wp-abilities-v1-api-openapi.yml
- filename: local-infusion-root-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Root API
  slug: local-infusion-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-root-api-openapi.yml
- filename: local-infusion-oembed-1-0-api-openapi.yml
  format: yaml
  label: Local Infusion oEmbed API
  slug: local-infusion-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-oembed-1-0-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Local Infusion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Local Infusion secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Local Infusion
provider_slug: local-infusion
scheme_count: 2
schemes:
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched 2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://mylocalinfusion.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://mylocalinfusion.com/oauth/token
  name: mcpOAuth2
  sources:
  - openapi/local-infusion-mcp-api-openapi.yml
  - openapi/local-infusion-oembed-1-0-api-openapi.yml
  - openapi/local-infusion-root-api-openapi.yml
  - openapi/local-infusion-wp-abilities-v1-api-openapi.yml
  - openapi/local-infusion-wp-v2-api-openapi.yml
  type: oauth2
- description: WordPress cookie-authentication nonce. Advertised by the live server in its Access-Control-Allow-Headers response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type), observed on a 401 from the MCP endpoint.
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/local-infusion-mcp-api-openapi.yml
  - openapi/local-infusion-oembed-1-0-api-openapi.yml
  - openapi/local-infusion-root-api-openapi.yml
  - openapi/local-infusion-wp-abilities-v1-api-openapi.yml
  - openapi/local-infusion-wp-v2-api-openapi.yml
  type: apiKey
slug: local-infusion-authentication
source_filename: local-infusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/local-infusion-mcp-api-openapi.yml, openapi/local-infusion-oembed-1-0-api-openapi.yml,\n  openapi/local-infusion-root-api-openapi.yml, openapi/local-infusion-wp-abilities-v1-api-openapi.yml,\n  openapi/local-infusion-wp-v2-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: mcpOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mylocalinfusion.com/oauth/authorize\n    tokenUrl: https://mylocalinfusion.com/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched\n    2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata\n    names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.\n\
  \  sources:\n  - openapi/local-infusion-mcp-api-openapi.yml\n  - openapi/local-infusion-oembed-1-0-api-openapi.yml\n  - openapi/local-infusion-root-api-openapi.yml\n  - openapi/local-infusion-wp-abilities-v1-api-openapi.yml\n  - openapi/local-infusion-wp-v2-api-openapi.yml\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie-authentication nonce. Advertised by the live server in its Access-Control-Allow-Headers\n    response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type),\n    observed on a 401 from the MCP endpoint.\n  sources:\n  - openapi/local-infusion-mcp-api-openapi.yml\n  - openapi/local-infusion-oembed-1-0-api-openapi.yml\n  - openapi/local-infusion-root-api-openapi.yml\n  - openapi/local-infusion-wp-abilities-v1-api-openapi.yml\n  - openapi/local-infusion-wp-v2-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/authentication/local-infusion-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health Services
- Infusion Therapy
- Specialty Pharmacy
- Ambulatory Care
- Patient Services
- Autoimmune
- Chronic Care
- MCP
- WordPress
---
