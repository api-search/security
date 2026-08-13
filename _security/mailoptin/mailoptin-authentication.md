---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Mailoptin Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailOptin declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MailOptin
provider_slug: mailoptin
scheme_count: 3
schemes:
- applies_to: https://mailoptin.io/wp-json/mcp/mcp-oauth-server
  authorization_url: https://mailoptin.io/oauth/authorize
  bearer_methods:
  - header
  client_registration: client_id_metadata_document
  evidence:
    http_status: 200
    url: https://mailoptin.io/.well-known/oauth-authorization-server
  flow: authorization_code
  id: oauth2_mcp
  issuer: https://mailoptin.io
  pkce: required
  pkce_methods:
  - S256
  refresh: true
  revocation_url: https://mailoptin.io/oauth/revoke
  scopes:
  - mcp
  token_endpoint_auth_methods:
  - none
  token_url: https://mailoptin.io/oauth/token
  type: oauth2
- applies_to: https://mailoptin.io/wp-json/
  authorization_url: https://mailoptin.io/wp-admin/authorize-application.php
  description: WordPress Application Passwords. The site's REST API root advertises the authorization endpoint in its `authentication` block. Per-user credentials issued from wp-admin; used with HTTP Basic.
  evidence:
    http_status: 200
    url: https://mailoptin.io/wp-json/
  id: application_passwords
  scheme: basic
  type: http
- applies_to: https://mailoptin.io/wp-json/
  description: WordPress cookie + nonce authentication for same-origin browser requests. Advertised in the CORS `access-control-allow-headers` response header alongside Authorization.
  evidence:
    http_status: 200
    url: https://mailoptin.io/wp-json/wp/v2/posts
  id: cookie_nonce
  in: header
  name: X-WP-Nonce
  type: apiKey
slug: mailoptin-authentication
source_filename: mailoptin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://mailoptin.io/.well-known/oauth-authorization-server,\n  https://mailoptin.io/.well-known/oauth-protected-resource,\n  https://mailoptin.io/wp-json/ (authentication block)\ndocs: https://mailoptin.io/docs/\nnote: >-\n  There is no OpenAPI to derive from — derive-authentication.py found no spec. This\n  profile is built entirely from documents mailoptin.io actually serves and from live\n  401 responses observed on 2026-08-12.\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  applies_to: https://mailoptin.io/wp-json/mcp/mcp-oauth-server\n  flow: authorization_code\n  pkce: required\n  pkce_methods: [S256]\n  issuer: https://mailoptin.io\n  authorization_url: https://mailoptin.io/oauth/authorize\n  token_url: https://mailoptin.io/oauth/token\n  revocation_url: https://mailoptin.io/oauth/revoke\n  refresh: true\n  scopes: [mcp]\n  token_endpoint_auth_methods: [none]\n  client_registration: client_id_metadata_document\n\
  \  bearer_methods: [header]\n  evidence:\n    url: https://mailoptin.io/.well-known/oauth-authorization-server\n    http_status: 200\n- id: application_passwords\n  type: http\n  scheme: basic\n  applies_to: https://mailoptin.io/wp-json/\n  description: >-\n    WordPress Application Passwords. The site's REST API root advertises the\n    authorization endpoint in its `authentication` block. Per-user credentials issued\n    from wp-admin; used with HTTP Basic.\n  authorization_url: https://mailoptin.io/wp-admin/authorize-application.php\n  evidence:\n    url: https://mailoptin.io/wp-json/\n    http_status: 200\n- id: cookie_nonce\n  type: apiKey\n  in: header\n  name: X-WP-Nonce\n  applies_to: https://mailoptin.io/wp-json/\n  description: >-\n    WordPress cookie + nonce authentication for same-origin browser requests. Advertised\n    in the CORS `access-control-allow-headers` response header alongside Authorization.\n  evidence:\n    url: https://mailoptin.io/wp-json/wp/v2/posts\n    http_status:\
  \ 200\nanonymous_access:\n  available: true\n  note: >-\n    Read-only content routes under /wp-json/wp/v2/ answer anonymously (posts returned\n    x-wp-total 260 on 2026-08-12). Write routes, the Abilities API and both MCP servers\n    are gated.\nobserved_denials:\n- url: https://mailoptin.io/wp-json/mcp/mcp-oauth-server\n  http_status: 401\n  code: mcp_unauthorized\n- url: https://mailoptin.io/wp-json/wp-abilities/v1/abilities\n  http_status: 401\n  code: rest_forbidden\nproduct_authentication:\n  note: >-\n    The MailOptin PRODUCT is a self-hosted WordPress plugin. It authenticates OUTBOUND to\n    60+ third-party email/CRM providers using each provider's own credentials (API keys,\n    OAuth). Those are the third parties' schemes, not MailOptin's, and are not recorded\n    here. MailOptin itself issues a license key, entered in wp-admin, for updates and\n    premium features.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailoptin/refs/heads/main/authentication/mailoptin-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Email Marketing
- Marketing Automation
- Lead Generation
- WordPress
- Newsletters
- Webhooks
- Model Context Protocol
- Plugins
---
