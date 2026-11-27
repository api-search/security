---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ConferenceGrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConferenceGrid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ConferenceGrid
provider_slug: conferencegrid-com
scheme_count: 1
schemes:
- authorization_url: https://conferencegrid.com/oauth/authorize
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  evidence: '"Anything else that speaks Streamable HTTP and OAuth 2.1 with PKCE works too." and "Sign in once with your free ConferenceGrid account; there is no API key to manage." (https://conferencegrid.com/mcp); values read from the two well-known metadata documents (GET, HTTP 200).'
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  metadata:
    authorization_server: https://conferencegrid.com/.well-known/oauth-authorization-server
    protected_resource: https://conferencegrid.com/.well-known/oauth-protected-resource
  name: oauth2
  pkce: S256
  registration_url: https://conferencegrid.com/api/oauth/register
  scopes:
  - conferences:read
  token_endpoint_auth_methods:
  - none
  token_notes: Tokens are audience-bound to the MCP endpoint; disconnecting the connector stops the token working within the hour (per /mcp).
  token_url: https://conferencegrid.com/api/oauth/token
  type: oauth2
slug: conferencegrid-com-authentication
source_filename: conferencegrid-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://conferencegrid.com/mcp\ndocs: https://conferencegrid.com/mcp\nsummary: The only programmatic surface is the remote MCP server at https://conferencegrid.com/api/mcp. It uses OAuth 2.1 authorization code with PKCE (S256), public clients (token_endpoint_auth_methods_supported none), dynamic client registration or a client metadata document URL, and a single scope conferences:read. No API key exists. An unauthenticated call returns 401 naming the protected resource metadata.\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorization_url: https://conferencegrid.com/oauth/authorize\n  token_url: https://conferencegrid.com/api/oauth/token\n  registration_url: https://conferencegrid.com/api/oauth/register\n  scopes:\n  - conferences:read\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - none\n  client_id_metadata_document_supported: true\n\
  \  bearer_methods:\n  - header\n  metadata:\n    authorization_server: https://conferencegrid.com/.well-known/oauth-authorization-server\n    protected_resource: https://conferencegrid.com/.well-known/oauth-protected-resource\n  evidence: '\"Anything else that speaks Streamable HTTP and OAuth 2.1 with PKCE works too.\" and \"Sign in once with your free ConferenceGrid account; there is no API key to manage.\" (https://conferencegrid.com/mcp); values read from the two well-known metadata documents (GET, HTTP 200).'\n  token_notes: Tokens are audience-bound to the MCP endpoint; disconnecting the connector stops the token working within the hour (per /mcp).\n"
source_yaml_url: https://artifacts.apis.io/conferencegrid-com/authentication/conferencegrid-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Conferences
- Event
- Trade Shows
- Sales Intelligence
- B2B
- Sponsorship
- MCP
---
