---
api_key_in: []
api_specs:
- filename: turntide-technologies-wordpress-rest-openapi.yml
  format: yaml
  label: Turntide WordPress REST API
  slug: turntide-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turntide-technologies/refs/heads/main/openapi/turntide-technologies-wordpress-rest-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Turntide Technologies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Turntide Technologies secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Turntide Technologies
provider_slug: turntide-technologies
scheme_count: 2
schemes:
- description: WordPress Application Passwords, advertised by the route index at https://turntide.com/wp-json/ under authentication.application-passwords; authorization endpoint https://turntide.com/wp-admin/authorize-application.php
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/turntide-technologies-wordpress-rest-openapi.yml
  type: http
- description: OAuth 2.1 authorization server advertised at https://turntide.com/.well-known/oauth-authorization-server (PKCE S256, scope 'mcp'); protects the MCP endpoint declared at https://turntide.com/.well-known/oauth-protected-resource
  flows:
  - authorizationUrl: https://turntide.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://turntide.com/oauth/token
  name: mcpOAuth2
  sources:
  - openapi/turntide-technologies-wordpress-rest-openapi.yml
  type: oauth2
slug: turntide-technologies-authentication
source_filename: turntide-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/turntide-technologies-wordpress-rest-openapi.yml\ndocs: https://turntide.com/.well-known/oauth-authorization-server\nx-evidence:\n  fetched: '2026-08-02'\n  application_passwords: >-\n    advertised at https://turntide.com/wp-json/ under authentication.application-passwords\n    (HTTP 200); authorize endpoint https://turntide.com/wp-admin/authorize-application.php\n  oauth2: >-\n    RFC 8414 metadata at https://turntide.com/.well-known/oauth-authorization-server (HTTP 200):\n    authorization code + refresh_token grants, PKCE S256 required, public clients\n    (token_endpoint_auth_methods_supported [\"none\"]), client_id_metadata_document_supported true,\n    revocation endpoint https://turntide.com/oauth/revoke\n  observed_401s:\n  - {url: 'https://turntide.com/wp-json/wp-abilities/v1/abilities', code: rest_forbidden, status: 401}\n  - {url: 'https://turntide.com/wp-json/mcp/mcp-oauth-server', code: mcp_unauthorized,\
  \ status: 401}\n  anonymous_read: 'wp/v2 published content collections read without credentials (HTTP 200)'\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the route index at https://turntide.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://turntide.com/wp-admin/authorize-application.php\n  sources:\n  - openapi/turntide-technologies-wordpress-rest-openapi.yml\n- name: mcpOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://turntide.com/oauth/authorize\n    tokenUrl: https://turntide.com/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization server advertised at https://turntide.com/.well-known/oauth-authorization-server\n    (PKCE S256, scope 'mcp'); protects the MCP endpoint declared at https://turntide.com/.well-known/oauth-protected-resource\n\
  \  sources:\n  - openapi/turntide-technologies-wordpress-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turntide-technologies/refs/heads/main/authentication/turntide-technologies-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Electrification
- Electric Motors
- Power Electronics
- Energy Storage
- Thermal Management
- Industrial Equipment
- Manufacturing
- Sustainability
- Building Automation
- Content Management
---
