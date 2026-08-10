---
api_key_in: []
auth_types: []
description: Derived entirely from anonymously-readable discovery metadata and live challenge responses on tunetx.com. Tune Therapeutics publishes no authentication documentation of any kind — there is no developer portal, no auth guide, and no reference page. Everything below was read off the wire from the OAuth 2.1 authorization server and the WordPress REST API that the site's plugins expose.
kind: authentication
layout: security
method: probed
name: Tune Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tune Therapeutics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tune Therapeutics
provider_slug: tune-therapeutics
scheme_count: 2
schemes:
- applies_to:
  - https://tunetx.com/wp-json/mcp/mcp-oauth-server
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  flows:
    authorizationCode:
      authorizationUrl: https://tunetx.com/oauth/authorize
      refreshUrl: https://tunetx.com/oauth/token
      revocationUrl: https://tunetx.com/oauth/revoke
      scopes:
        mcp: The only scope the authorization server advertises. Grants access to the MCP server; its concrete permission surface is not documented publicly.
      tokenUrl: https://tunetx.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: mcp_oauth2
  issuer: https://tunetx.com
  metadata_spec: RFC 8414
  metadata_url: https://tunetx.com/.well-known/oauth-authorization-server/
  name: WordPress MCP OAuth 2.1
  observations:
  - PKCE with S256 is the only code-challenge method offered, and the token endpoint accepts no client authentication — the modern OAuth 2.1 public-client shape.
  - client_id_metadata_document_supported is true, meaning clients may identify themselves with a URL-hosted client metadata document rather than pre-registering.
  - A bare POST to the token endpoint returns HTTP 400 {"error":"unsupported_grant_type"} — a real, correctly-behaving OAuth token endpoint, not a stub.
  pkce_required: true
  protected_resource_metadata_spec: RFC 9728
  protected_resource_metadata_url: https://tunetx.com/.well-known/oauth-protected-resource
  public_client: true
  response_types_supported:
  - code
  token_endpoint_auth_methods_supported:
  - none
  token_placement: 'Authorization: Bearer <token>'
  type: oauth2
- applies_to:
  - https://tunetx.com/wp-json/
  authorization_url: https://tunetx.com/wp-admin/authorize-application.php
  id: wp_application_passwords
  name: WordPress Application Passwords
  note: Advertised in the WordPress REST API index as the site's supported authentication method for the wp/v2 and adapter routes. Credentials are issued from wp-admin, so this is a site-operator mechanism, not a public developer credential.
  scheme: basic
  source: https://tunetx.com/wp-json/ → authentication.application-passwords
  type: http
slug: tune-therapeutics-authentication
source_filename: tune-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://tunetx.com/.well-known/oauth-authorization-server/\nname: Tune Therapeutics — authentication profile\ndescription: >-\n  Derived entirely from anonymously-readable discovery metadata and live challenge\n  responses on tunetx.com. Tune Therapeutics publishes no authentication documentation of\n  any kind — there is no developer portal, no auth guide, and no reference page. Everything\n  below was read off the wire from the OAuth 2.1 authorization server and the WordPress\n  REST API that the site's plugins expose.\n\ndocs: null\ndocs_note: >-\n  No authentication documentation exists to link. The provider could close this by\n  publishing an auth page, but there is no product API for it to describe.\n\nschemes:\n\n- id: mcp_oauth2\n  type: oauth2\n  name: WordPress MCP OAuth 2.1\n  applies_to:\n  - https://tunetx.com/wp-json/mcp/mcp-oauth-server\n  issuer: https://tunetx.com\n  metadata_url: https://tunetx.com/.well-known/oauth-authorization-server/\n\
  \  metadata_spec: RFC 8414\n  protected_resource_metadata_url: https://tunetx.com/.well-known/oauth-protected-resource\n  protected_resource_metadata_spec: RFC 9728\n  flows:\n    authorizationCode:\n      authorizationUrl: https://tunetx.com/oauth/authorize\n      tokenUrl: https://tunetx.com/oauth/token\n      refreshUrl: https://tunetx.com/oauth/token\n      revocationUrl: https://tunetx.com/oauth/revoke\n      scopes:\n        mcp: >-\n          The only scope the authorization server advertises. Grants access to the MCP\n          server; its concrete permission surface is not documented publicly.\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  pkce_required: true\n  token_endpoint_auth_methods_supported: [none]\n  public_client: true\n  client_id_metadata_document_supported: true\n  token_placement: 'Authorization: Bearer <token>'\n  observations:\n  - >-\n    PKCE with S256 is the only\
  \ code-challenge method offered, and the token endpoint\n    accepts no client authentication — the modern OAuth 2.1 public-client shape.\n  - >-\n    client_id_metadata_document_supported is true, meaning clients may identify themselves\n    with a URL-hosted client metadata document rather than pre-registering.\n  - >-\n    A bare POST to the token endpoint returns HTTP 400 {\"error\":\"unsupported_grant_type\"} —\n    a real, correctly-behaving OAuth token endpoint, not a stub.\n\n- id: wp_application_passwords\n  type: http\n  scheme: basic\n  name: WordPress Application Passwords\n  applies_to:\n  - https://tunetx.com/wp-json/\n  authorization_url: https://tunetx.com/wp-admin/authorize-application.php\n  source: 'https://tunetx.com/wp-json/ → authentication.application-passwords'\n  note: >-\n    Advertised in the WordPress REST API index as the site's supported authentication\n    method for the wp/v2 and adapter routes. Credentials are issued from wp-admin, so this\n    is a site-operator\
  \ mechanism, not a public developer credential.\n\nanonymous_access:\n- surface: https://tunetx.com/wp-json/wp/v2/posts\n  status: 200\n  note: >-\n    Public read of published site content is open, as on any default WordPress install.\n    No credential is required to read the marketing site's posts through the REST API.\n- surface: https://tunetx.com/wp-json/\n  status: 200\n  note: 432 routes across 23 namespaces enumerable anonymously.\n\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://tunetx.com/.well-known/oauth-authorization-server/\n    status: 200\n  - url: https://tunetx.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://tunetx.com/oauth/token\n    method: POST\n    status: 400\n    body: '{\"error\":\"unsupported_grant_type\"}'\n  - url: https://tunetx.com/oauth/authorize\n    status: 301\n  - url: https://tunetx.com/wp-json/\n    status: 200\n  - url: https://tunetx.com/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tune-therapeutics/refs/heads/main/authentication/tune-therapeutics-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Therapeutics
- Genomics
- Epigenetics
- Gene Therapy
- Clinical Stage
- Research
---
