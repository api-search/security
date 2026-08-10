---
api_key_in:
- header
api_specs:
- filename: a2-biotherapeutics-mcp-api-openapi.yml
  format: yaml
  label: A2 Biotherapeutics MCP API
  slug: a2-biotherapeutics-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-mcp-api-openapi.yml
- filename: a2-biotherapeutics-oembed-1-0-api-openapi.yml
  format: yaml
  label: A2 Biotherapeutics Oembed/1.0 API
  slug: a2-biotherapeutics-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-oembed-1-0-api-openapi.yml
- filename: a2-biotherapeutics-root-api-openapi.yml
  format: yaml
  label: A2 Biotherapeutics Root API
  slug: a2-biotherapeutics-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-root-api-openapi.yml
- filename: a2-biotherapeutics-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: A2 Biotherapeutics Wp Abilities/v1 API
  slug: a2-biotherapeutics-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-wp-abilities-v1-api-openapi.yml
- filename: a2-biotherapeutics-wp-v2-api-openapi.yml
  format: yaml
  label: A2 Biotherapeutics Wp/v2 API
  slug: a2-biotherapeutics-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-wp-v2-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: A2 Biotherapeutics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: A2 Biotherapeutics secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: A2 Biotherapeutics
provider_slug: a2-biotherapeutics
scheme_count: 2
schemes:
- description: OAuth 2.1 authorization-code + PKCE, as advertised by the provider's RFC 8414 metadata at https://www.a2bio.com/.well-known/oauth-authorization-server (fetched 2026-08-02, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://www.a2bio.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://www.a2bio.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://www.a2bio.com/oauth/token
  name: mcpOAuth2
  sources:
  - openapi/a2-biotherapeutics-wp-rest-openapi.yml
  type: oauth2
- description: WordPress cookie-authentication nonce. Advertised by the live server in its Access-Control-Allow-Headers response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).
  in: header
  name: wpNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/a2-biotherapeutics-wp-rest-openapi.yml
  type: apiKey
slug: a2-biotherapeutics-authentication
source_filename: a2-biotherapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/a2-biotherapeutics-wp-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: mcpOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.a2bio.com/oauth/authorize\n    tokenUrl: https://www.a2bio.com/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization-code + PKCE, as advertised by the provider's RFC 8414\n    metadata at https://www.a2bio.com/.well-known/oauth-authorization-server (fetched 2026-08-02,\n    HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names\n    https://www.a2bio.com/wp-json/mcp/mcp-oauth-server.\n  sources:\n  - openapi/a2-biotherapeutics-wp-rest-openapi.yml\n- name: wpNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie-authentication nonce. Advertised by the live server in its\
  \ Access-Control-Allow-Headers\n    response header (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).\n  sources:\n  - openapi/a2-biotherapeutics-wp-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/authentication/a2-biotherapeutics-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Immuno-Oncology
- Oncology
- Pharmaceuticals
- Clinical Trials
- Healthcare
- Model Context Protocol
- WordPress
---
