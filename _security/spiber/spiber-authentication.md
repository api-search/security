---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Spiber Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spiber declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Spiber
provider_slug: spiber
scheme_count: 3
schemes:
- authorization_endpoint: https://spiber.xsrv.jp/api/wp-admin/authorize-application.php
  description: WordPress Application Passwords. Declared by the service in its own discovery document under authentication.application-passwords.
  documented_by_provider: false
  evidence: authentication.application-passwords.endpoints.authorization in the wp-json root
  id: application-passwords
  scheme: basic
  type: http
- bearer_format: JWT
  description: A JWT namespace is registered on the service (jwt-auth/v1 with /token and /token/validate routes). Token issuance requires WordPress credentials; no public registration exists.
  documented_by_provider: false
  evidence: namespaces[] includes "jwt-auth/v1" in the wp-json root discovery document
  id: jwt-auth
  scheme: bearer
  token_endpoint: https://spiber.xsrv.jp/api/wp-json/jwt-auth/v1/token
  type: http
  validate_endpoint: https://spiber.xsrv.jp/api/wp-json/jwt-auth/v1/token/validate
- description: Cookie authentication with an X-WP-Nonce header, used by the site's own front end. Not available to third parties.
  documented_by_provider: false
  evidence: Access-Control-Allow-Headers on every response lists Authorization, X-WP-Nonce
  id: cookie-nonce
  in: header
  name: X-WP-Nonce
  type: apiKey
slug: spiber-authentication
source_filename: spiber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://spiber.xsrv.jp/api/wp-json/ (WordPress REST discovery document, HTTP 200)\nnote: >-\n  Spiber publishes no authentication documentation because it publishes no developer program.\n  This profile is read directly off the live WordPress REST discovery document the service serves\n  about itself, plus observed anonymous responses. Public content reads require no credential at\n  all; everything else is permission-gated behind WordPress capabilities. There is no OAuth 2.0\n  authorization server, no OpenID Connect discovery document, and no API-key issuance surface.\napi: spiber-content-api\nbase_url: https://spiber.xsrv.jp/api/wp-json\nanonymous_access:\n  supported: true\n  scope: read-only access to published content routes (wp/v2 posts, pages, media, types,\n    taxonomies, and the custom/v1 menus and news listings)\n  evidence: 'GET /wp/v2/pages?per_page=1 returned HTTP 200 with X-WP-Total: 20 and no credential'\nschemes:\n\
  - id: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords. Declared by the service in its own discovery document under\n    authentication.application-passwords.\n  authorization_endpoint: https://spiber.xsrv.jp/api/wp-admin/authorize-application.php\n  evidence: authentication.application-passwords.endpoints.authorization in the wp-json root\n  documented_by_provider: false\n- id: jwt-auth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    A JWT namespace is registered on the service (jwt-auth/v1 with /token and /token/validate\n    routes). Token issuance requires WordPress credentials; no public registration exists.\n  token_endpoint: https://spiber.xsrv.jp/api/wp-json/jwt-auth/v1/token\n  validate_endpoint: https://spiber.xsrv.jp/api/wp-json/jwt-auth/v1/token/validate\n  evidence: namespaces[] includes \"jwt-auth/v1\" in the wp-json root discovery document\n  documented_by_provider: false\n- id: cookie-nonce\n\
  \  type: apiKey\n  in: header\n  name: X-WP-Nonce\n  description: >-\n    Cookie authentication with an X-WP-Nonce header, used by the site's own front end. Not\n    available to third parties.\n  evidence: 'Access-Control-Allow-Headers on every response lists Authorization, X-WP-Nonce'\n  documented_by_provider: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiber/refs/heads/main/authentication/spiber-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Biotechnology
- Materials Science
- Synthetic Biology
- Manufacturing
- Sustainability
- Textiles
- Precision Fermentation
- Japan
- Content
---
