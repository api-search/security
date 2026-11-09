---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dimensionkit Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DimensionKit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DimensionKit
provider_slug: dimensionkit-com
scheme_count: 1
schemes:
- applies_to: https://app.dimensionkit.com/mcp
  bearer_methods:
  - header
  description: OAuth 2.1, authorization code with PKCE. Dynamic client registration (RFC 7591) is open, which is what makes pasting the URL enough. Nothing is issued by hand - there are no API keys to copy.
  discovery:
    authorization_server_metadata: https://app.dimensionkit.com/.well-known/oauth-authorization-server
    note: The 401 from /mcp carries a WWW-Authenticate header whose resource_metadata parameter points at the RFC 9728 document.
    protected_resource_metadata: https://app.dimensionkit.com/.well-known/oauth-protected-resource
  flows:
    authorizationCode:
      grant_types:
      - authorization_code
      - refresh_token
      issuer: https://app.dimensionkit.com
      pkce: S256
      registrationUrl: https://app.dimensionkit.com/oauth/register
      revocationUrl: https://app.dimensionkit.com/oauth/revoke
      scopes:
        scorecards:read: View your scorecards, their configuration, and submissions
        scorecards:write: Create, edit, and publish your scorecards
      token_endpoint_auth_methods:
      - none
      - client_secret_post
      - client_secret_basic
  name: oauth2
  prerequisites: Email verification is required before a connector can be approved.
  redirect_uris: https:// , custom schemes such as cursor:// , and http:// for loopback addresses only
  revocation: RFC 7009 at /oauth/revoke; revoking either token revokes both halves of the grant
  token_lifetimes:
    access_token: 1 hour
    refresh_token: 30 days (rotating; each refresh issues a new refresh token)
  type: oauth2
slug: dimensionkit-com-authentication
source_filename: dimensionkit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dimensionkit.com/docs/mcp/connecting/\ndocs: https://dimensionkit.com/docs/mcp/connecting/\nname: DimensionKit authentication\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://app.dimensionkit.com/mcp\n  description: 'OAuth 2.1, authorization code with PKCE. Dynamic client registration (RFC 7591) is open, which is what makes pasting the URL enough. Nothing is issued by hand - there are no API keys to copy.'\n  flows:\n    authorizationCode:\n      issuer: https://app.dimensionkit.com\n      registrationUrl: https://app.dimensionkit.com/oauth/register\n      revocationUrl: https://app.dimensionkit.com/oauth/revoke\n      pkce: S256\n      grant_types: [authorization_code, refresh_token]\n      token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n      scopes:\n        scorecards:read: View your scorecards, their configuration, and submissions\n        scorecards:write: Create,\
  \ edit, and publish your scorecards\n  bearer_methods: [header]\n  discovery:\n    protected_resource_metadata: https://app.dimensionkit.com/.well-known/oauth-protected-resource\n    authorization_server_metadata: https://app.dimensionkit.com/.well-known/oauth-authorization-server\n    note: The 401 from /mcp carries a WWW-Authenticate header whose resource_metadata parameter points at the RFC 9728 document.\n  token_lifetimes:\n    access_token: 1 hour\n    refresh_token: 30 days (rotating; each refresh issues a new refresh token)\n  redirect_uris: https:// , custom schemes such as cursor:// , and http:// for loopback addresses only\n  revocation: RFC 7009 at /oauth/revoke; revoking either token revokes both halves of the grant\n  prerequisites: Email verification is required before a connector can be approved.\nevidence:\n- url: https://app.dimensionkit.com/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://app.dimensionkit.com/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n- url: https://dimensionkit.com/docs/mcp/managing/\n"
source_yaml_url: https://artifacts.apis.io/dimensionkit-com/authentication/dimensionkit-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Assessment
- Scorecards
- Lead Generation
- MCP
- Artificial Intelligence
- Quizzes
---
