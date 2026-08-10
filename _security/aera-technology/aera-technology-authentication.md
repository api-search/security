---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Aera Technology Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aera Technology secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aera Technology
provider_slug: aera-technology
scheme_count: 1
schemes:
- bearerMethods:
  - header
  clientIdMetadataDocumentSupported: true
  flows:
  - authorizationUrl: https://www.aeratechnology.com/oauth/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    refreshSupported: true
    revocationUrl: https://www.aeratechnology.com/oauth/revoke
    scopes:
      mcp: Access the Aera Technology MCP server
    tokenUrl: https://www.aeratechnology.com/oauth/token
  issuer: https://www.aeratechnology.com
  name: mcp-oauth
  sources:
  - well-known/aera-technology-oauth-authorization-server.json
  - well-known/aera-technology-oauth-protected-resource.json
  tokenEndpointAuthMethods:
  - none
  type: oauth2
slug: aera-technology-authentication
source_filename: aera-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://www.aeratechnology.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the live RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata Aera Technology publishes on www.aeratechnology.com.\n  There is no public OpenAPI to derive securitySchemes from — the Aera Decision\n  Cloud reference is behind a customer SSO login — so this profile covers only the\n  publicly discoverable MCP authorization surface.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  public_client: true\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  issuer: https://www.aeratechnology.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.aeratechnology.com/oauth/authorize\n    tokenUrl: https://www.aeratechnology.com/oauth/token\n    revocationUrl: https://www.aeratechnology.com/oauth/revoke\n    refreshSupported: true\n    codeChallengeMethods:\
  \ [S256]\n    scopes:\n      mcp: Access the Aera Technology MCP server\n  tokenEndpointAuthMethods: [none]\n  clientIdMetadataDocumentSupported: true\n  bearerMethods: [header]\n  sources:\n  - well-known/aera-technology-oauth-authorization-server.json\n  - well-known/aera-technology-oauth-protected-resource.json\nprotected_resources:\n- resource: https://www.aeratechnology.com/wp-json/mcp/mcp-oauth-server\n  authorization_servers: [https://www.aeratechnology.com]\n  scopes: [mcp]\ngated:\n- surface: Aera Decision Cloud product API\n  docs: https://docs.aeratechnology.com/\n  status: 302\n  note: >-\n    Redirects to idp-dev.aeratechnology.com (Aera's identity provider). The\n    Document360 documentation site requires a customer login, so the product API's\n    authentication model is not publicly documented and is deliberately NOT\n    described here.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://www.aeratechnology.com/.well-known/oauth-authorization-server\n  \
  \  http_status: 200\n  - url: https://www.aeratechnology.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://docs.aeratechnology.com/\n    http_status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aera-technology/refs/heads/main/authentication/aera-technology-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Decision Intelligence
- Artificial Intelligence
- Enterprise Software
- Supply Chain
- Automation
- Analytics
- Agents
---
