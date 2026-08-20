---
api_key_in:
- header
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Reso Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: RESO (Real Estate Standards Organization) secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: RESO (Real Estate Standards Organization)
provider_slug: reso
scheme_count: 3
schemes:
- applies_to: RESO-certified Web API servers (any MLS or data provider)
  issuer: The individual MLS or its software provider. RESO issues no Web API credentials.
  name: OAuth2 Bearer Token
  required: true
  scheme: bearer
  spec: Web API Core 2.0.0/2.1.0 (RCP-37), section on Authentication; RCP-WEBAPI-026
  spec_text: '"Providers MUST use either OAuth2 Bearer tokens or Client Credentials for authentication (RCP-026)."'
  type: http
- applies_to: RESO-certified Web API servers (any MLS or data provider)
  flow: clientCredentials
  name: OAuth2 Client Credentials
  parameters:
  - client_id
  - client_secret
  required: true
  spec: Web API Core 2.0.0/2.1.0 (RCP-37)
  spec_text: '"A type of authorization grant that uses a client_id and client_secret ... in order to provide a Bearer Token upon request. This method is more resilient against man-in-the-middle attacks than Bearer Tokens since there is an additional token request step involved, and tokens may be expired and refreshed programmatically."'
  token_url: Provider-specific - each MLS publishes its own token endpoint. RESO defines no central one.
  type: oauth2
- applies_to: https://services.reso.org/mcp
  format: Bearer <api-key>
  how_to_obtain: Email dev@reso.org with name, organization and intended use case (development, testing, demo, integration). Beta programme; keys available to RESO members and conference attendees.
  in: header
  issuer: RESO
  name: RESO Cloud MCP API key
  parameter: Authorization
  probe:
    anonymous_status: 401
    date: '2026-07-26'
    url: https://services.reso.org/mcp
  required: true
  self_serve: false
  type: apiKey
slug: reso-authentication
source_filename: reso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://github.com/RESOStandards/transport/blob/main/proposals/web-api-core.md\nsource:\n- https://github.com/RESOStandards/transport/blob/main/proposals/web-api-core.md\n- https://github.com/RESOStandards/reso-tools/blob/main/reso-mcp-server/doc/GUIDE.md\n- https://github.com/RESOStandards/reso-tools/blob/main/reso-certification/README.md\nnote: >-\n  Two authentication stories that must be held apart. (1) The auth model RESO MANDATES for every\n  RESO-certified Web API server - OAuth2 Bearer tokens or OAuth2 Client Credentials over TLS 1.2+,\n  with credentials issued by the individual MLS, never by RESO. (2) The auth on the one endpoint\n  RESO itself operates - the RESO Cloud MCP Server at services.reso.org/mcp, which gates on a\n  static bearer API key issued by RESO on request. Derived from OpenAPI securitySchemes was not\n  possible: RESO publishes no OpenAPI, so this profile is transcribed from the ratified\n  specification\
  \ text.\nsummary:\n  types: [oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  transport_security: TLS 1.2 or above (mandatory)\n  openid_connect: >-\n    Removed. \"The Open ID Connect layer was previously supported by the RESO Web API. As of\n    Web API 1.0.2, RESO only supports Bearer tokens and Client Credentials during Certification.\"\n  scopes_published: false\nschemes:\n- name: OAuth2 Bearer Token\n  type: http\n  scheme: bearer\n  applies_to: RESO-certified Web API servers (any MLS or data provider)\n  required: true\n  spec_text: >-\n    \"Providers MUST use either OAuth2 Bearer tokens or Client Credentials for authentication\n    (RCP-026).\"\n  spec: Web API Core 2.0.0/2.1.0 (RCP-37), section on Authentication; RCP-WEBAPI-026\n  issuer: The individual MLS or its software provider. RESO issues no Web API credentials.\n- name: OAuth2 Client Credentials\n  type: oauth2\n  flow: clientCredentials\n  applies_to: RESO-certified Web API servers (any MLS\
  \ or data provider)\n  required: true\n  token_url: Provider-specific - each MLS publishes its own token endpoint. RESO defines no central one.\n  parameters: [client_id, client_secret]\n  spec_text: >-\n    \"A type of authorization grant that uses a client_id and client_secret ... in order to provide a\n    Bearer Token upon request. This method is more resilient against man-in-the-middle attacks than\n    Bearer Tokens since there is an additional token request step involved, and tokens may be\n    expired and refreshed programmatically.\"\n  spec: Web API Core 2.0.0/2.1.0 (RCP-37)\n- name: RESO Cloud MCP API key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <api-key>'\n  applies_to: https://services.reso.org/mcp\n  required: true\n  issuer: RESO\n  how_to_obtain: >-\n    Email dev@reso.org with name, organization and intended use case (development, testing, demo,\n    integration). Beta programme; keys available to RESO members and conference attendees.\n\
  \  self_serve: false\n  probe: {url: 'https://services.reso.org/mcp', anonymous_status: 401, date: '2026-07-26'}\nclient_support:\n  reso_client_sdk:\n    package: '@reso-standards/reso-client'\n    supports: [bearer token, oauth2 client credentials]\n  reso_cert_cli:\n    package: '@reso-standards/reso-certification'\n    resolution_order:\n    - 'CLI flags: --auth-token, or --client-id / --client-secret / --token-url'\n    - 'Config file: --config path/to/config.json (per-entry auth)'\n    - '.env file in the current directory'\n    - 'Environment variables: RESO_AUTH_TOKEN, or RESO_CLIENT_ID / RESO_CLIENT_SECRET / RESO_TOKEN_URI'\n  web_api_commander:\n    language: java\n    supports: [bearer token, oauth2 client credentials]\nerror_semantics:\n  '403': Returned when the selected authentication mechanism is not successful (Web API Core section 2.6.1).\naccess_reality: >-\n  Authentication is standardised; access is not. A RESO-certified endpoint proves conformance to\n  this OAuth2\
  \ contract and proves nothing about reachability - credentials are issued only after a\n  data licence is signed with the individual MLS that runs the endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reso/refs/heads/main/authentication/reso-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Real-Estate
- United States
- RESO
- MLS
- Property Listings
- Data Standards
- OData
- Industry Body
- IDX
- PropTech
---
