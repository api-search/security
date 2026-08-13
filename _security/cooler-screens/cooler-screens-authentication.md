---
api_key_in: []
auth_types: []
description: CoolerX publishes no developer portal and no authentication documentation. This profile is read entirely from the two OAuth metadata documents the apex host serves and from the live 401 challenge returned by the MCP endpoint. It describes access to the coolerx.com WordPress MCP surface only. Access to the CoolerX retail-media platform (api.coolerx.com, portal.coolerx.com) is not documented anywhere public and those hosts refuse connections, so nothing is recorded about it.
kind: authentication
layout: security
method: probed
name: Cooler Screens Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoolerX declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CoolerX
provider_slug: cooler-screens
scheme_count: 2
schemes:
- applies_to: https://coolerx.com/wp-json/mcp/mcp-oauth-server
  authorization_url: https://coolerx.com/oauth/authorize
  challenge:
    note: RFC 9728 compliant — the challenge points at the protected-resource document.
    status: 401
    www_authenticate: Bearer realm="https://coolerx.com", resource_metadata="https://coolerx.com/.well-known/oauth-protected-resource"
  client_authentication:
  - none
  client_type: public
  dynamic_client_registration:
    client_id_metadata_document: true
    note: No registration_endpoint is advertised. The server instead declares client_id_metadata_document_supported, the newer OAuth Client ID Metadata Document pattern in which a client's URL is its client_id, so no registration call is made.
    rfc7591_endpoint: false
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2_mcp
  issuer: https://coolerx.com
  pkce:
    code_challenge_methods:
    - S256
    required: true
  response_types:
  - code
  revocation_url: https://coolerx.com/oauth/revoke
  scopes:
  - mcp
  token_delivery:
    header: Authorization
    location: header
    scheme: Bearer
  token_url: https://coolerx.com/oauth/token
  type: oauth2
- applies_to: https://coolerx.com/wp-json/ (WordPress REST API, including mcp-adapter-default-server)
  id: wordpress_application_password
  note: 'The WordPress REST root at https://coolerx.com/wp-json/ advertises authentication: {"application-passwords": ...}. This is stock WordPress credentialing for the marketing site''s CMS, not a CoolerX product credential. Listed for completeness; it is not a developer-facing API key programme.'
  scheme: basic
  type: http
slug: cooler-screens-authentication
source_filename: cooler-screens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://coolerx.com/.well-known/oauth-authorization-server\nname: CoolerX authentication profile\ndescription: >-\n  CoolerX publishes no developer portal and no authentication documentation. This\n  profile is read entirely from the two OAuth metadata documents the apex host serves\n  and from the live 401 challenge returned by the MCP endpoint. It describes access to\n  the coolerx.com WordPress MCP surface only. Access to the CoolerX retail-media\n  platform (api.coolerx.com, portal.coolerx.com) is not documented anywhere public and\n  those hosts refuse connections, so nothing is recorded about it.\nderived_from:\n- well-known/cooler-screens-oauth-authorization-server.json\n- well-known/cooler-screens-oauth-protected-resource.json\n- mcp/cooler-screens-mcp.yml\ndocs: null\ndocs_note: >-\n  No authentication or developer documentation exists on any CoolerX host. Probed\n  https://coolerx.com/developers/ (404), /developer/\
  \ (404), /api/ (404), /docs (404),\n  /api-docs (404) on 2026-08-12.\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  flow: authorizationCode\n  applies_to: https://coolerx.com/wp-json/mcp/mcp-oauth-server\n  issuer: https://coolerx.com\n  authorization_url: https://coolerx.com/oauth/authorize\n  token_url: https://coolerx.com/oauth/token\n  revocation_url: https://coolerx.com/oauth/revoke\n  response_types:\n  - code\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce:\n    required: true\n    code_challenge_methods:\n    - S256\n  client_authentication:\n  - none\n  client_type: public\n  dynamic_client_registration:\n    rfc7591_endpoint: false\n    client_id_metadata_document: true\n    note: >-\n      No registration_endpoint is advertised. The server instead declares\n      client_id_metadata_document_supported, the newer OAuth Client ID Metadata Document\n      pattern in which a client's URL is its client_id, so no registration call is made.\n  scopes:\n  - mcp\n \
  \ token_delivery:\n    location: header\n    scheme: Bearer\n    header: Authorization\n  challenge:\n    status: 401\n    www_authenticate: >-\n      Bearer realm=\"https://coolerx.com\",\n      resource_metadata=\"https://coolerx.com/.well-known/oauth-protected-resource\"\n    note: RFC 9728 compliant — the challenge points at the protected-resource document.\n- id: wordpress_application_password\n  type: http\n  scheme: basic\n  applies_to: https://coolerx.com/wp-json/ (WordPress REST API, including mcp-adapter-default-server)\n  note: >-\n    The WordPress REST root at https://coolerx.com/wp-json/ advertises\n    authentication: {\"application-passwords\": ...}. This is stock WordPress\n    credentialing for the marketing site's CMS, not a CoolerX product credential. Listed\n    for completeness; it is not a developer-facing API key programme.\nobservations:\n- no_api_keys_published: true\n- no_signup_or_key_issuance_page: true\n- oidc: false\n  note: /.well-known/openid-configuration\
  \ returns 404; the AS is OAuth 2.0 only.\n- mtls: false\ncaveat: >-\n  Every endpoint above is on coolerx.com, which serves a TLS certificate that expired\n  2025-06-10. A client that validates certificates cannot complete any of these flows.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooler-screens/refs/heads/main/authentication/cooler-screens-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Retail
- Retail Media
- Advertising
- Digital Signage
- In-Store Media
- Merchandising
- Artificial Intelligence
- Internet of Things
---
