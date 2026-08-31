---
api_key_in: []
auth_types: []
description: 'GigaIO publishes exactly one machine-readable authentication surface: the OAuth 2.0 authorization server backing its Model Context Protocol endpoint. Its FabreX/Gryf product APIs (DMTF Redfish) have no public authentication documentation — the reference sits behind the Atlassian-hosted customer support portal — so nothing about product-API auth is asserted here.'
kind: authentication
layout: security
method: probed
name: Gigaio Authentication
name_suffix: Authentication
oauth_flows: []
overview: GigaIO declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GigaIO
provider_slug: gigaio
scheme_count: 1
schemes:
- applies_to: https://gigaio.com/wp-json/mcp/mcp-oauth-server
  bearer_methods_supported:
  - header
  client_authentication:
    note: 'Public clients only — the token endpoint accepts no client secret. Client identity is established by a client-id metadata document (client_id_metadata_document_supported: true), so a client registers by publishing its own metadata URL rather than by pre-registering with GigaIO.'
    token_endpoint_auth_methods:
    - none
  evidence:
  - http_status: 200
    url: https://gigaio.com/.well-known/oauth-authorization-server
  - http_status: 200
    url: https://gigaio.com/.well-known/oauth-protected-resource
  - http_status: 401
    note: Anonymous POST returns mcp_unauthorized, confirming the resource is protected.
    url: https://gigaio.com/wp-json/mcp/mcp-oauth-server
  flows:
    authorization_code:
      authorizationUrl: https://gigaio.com/oauth/authorize
      refreshUrl: https://gigaio.com/oauth/token
      scopes:
        mcp: Access the GigaIO Model Context Protocol server.
      tokenUrl: https://gigaio.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp_oauth2
  issuer: https://gigaio.com
  pkce:
    code_challenge_methods:
    - S256
    required: true
  response_types:
  - code
  revocation_endpoint: https://gigaio.com/oauth/revoke
  rfc:
  - RFC 6749 (OAuth 2.0)
  - RFC 7636 (PKCE)
  - RFC 7009 (token revocation)
  - RFC 8414 (authorization server metadata)
  - RFC 9728 (protected resource metadata)
  type: oauth2
slug: gigaio-authentication
source_filename: gigaio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: https://gigaio.com/.well-known/oauth-authorization-server\ndescription: >-\n  GigaIO publishes exactly one machine-readable authentication surface: the OAuth 2.0\n  authorization server backing its Model Context Protocol endpoint. Its FabreX/Gryf\n  product APIs (DMTF Redfish) have no public authentication documentation — the\n  reference sits behind the Atlassian-hosted customer support portal — so nothing about\n  product-API auth is asserted here.\nschemes:\n  - id: mcp_oauth2\n    type: oauth2\n    applies_to: https://gigaio.com/wp-json/mcp/mcp-oauth-server\n    issuer: https://gigaio.com\n    flows:\n      authorization_code:\n        authorizationUrl: https://gigaio.com/oauth/authorize\n        tokenUrl: https://gigaio.com/oauth/token\n        refreshUrl: https://gigaio.com/oauth/token\n        scopes:\n          mcp: Access the GigaIO Model Context Protocol server.\n    grant_types: [authorization_code, refresh_token]\n\
  \    response_types: [code]\n    pkce:\n      required: true\n      code_challenge_methods: [S256]\n    client_authentication:\n      token_endpoint_auth_methods: [none]\n      note: >-\n        Public clients only — the token endpoint accepts no client secret. Client\n        identity is established by a client-id metadata document\n        (client_id_metadata_document_supported: true), so a client registers by\n        publishing its own metadata URL rather than by pre-registering with GigaIO.\n    revocation_endpoint: https://gigaio.com/oauth/revoke\n    bearer_methods_supported: [header]\n    rfc:\n      - RFC 6749 (OAuth 2.0)\n      - RFC 7636 (PKCE)\n      - RFC 7009 (token revocation)\n      - RFC 8414 (authorization server metadata)\n      - RFC 9728 (protected resource metadata)\n    evidence:\n      - url: https://gigaio.com/.well-known/oauth-authorization-server\n        http_status: 200\n      - url: https://gigaio.com/.well-known/oauth-protected-resource\n        http_status:\
  \ 200\n      - url: https://gigaio.com/wp-json/mcp/mcp-oauth-server\n        http_status: 401\n        note: Anonymous POST returns mcp_unauthorized, confirming the resource is protected.\nnot_documented:\n  - surface: FabreX fabric management (DMTF Redfish RESTful API)\n    reason: >-\n      GigaIO markets Redfish APIs for FabreX fabric management and an integration guide,\n      but publishes no public authentication reference. The knowledge base requires a\n      support-portal login and the CLI page directs readers to \"CONTACT US for details\n      on APIs\".\n    evidence:\n      - url: https://gigaio.com/products/fabrex-software/\n        http_status: 200\n      - url: https://gigaio.com/sign-in-to-gigaio-support/\n        http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigaio/refs/heads/main/authentication/gigaio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Composable Infrastructure
- Edge Computing
- Artificial Intelligence
- High Performance Computing
- Data-Center
- Hardware
- GPU
- PCIe
- Infrastructure as Code
---
