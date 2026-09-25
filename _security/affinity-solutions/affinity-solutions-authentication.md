---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Affinity Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affinity Solutions declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Affinity Solutions
provider_slug: affinity-solutions
scheme_count: 2
schemes:
- applies_to:
  - https://www.affinity.solutions/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://www.affinity.solutions/oauth/authorize
  client_registration:
    client_id_metadata_document_supported: true
    dynamic_registration_endpoint: null
    note: No RFC 7591 dynamic client registration endpoint is advertised. Instead the server declares client_id_metadata_document_supported, so a client identifies itself with a URL-shaped client_id resolving to its own metadata document. Public clients only (token_endpoint_auth_methods_supported is ["none"]), which is the OAuth 2.1 public-client-with-PKCE profile MCP expects.
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://www.affinity.solutions
  name: oauth2_mcp
  pkce:
    required_methods:
    - S256
  response_types_supported:
  - code
  revocation_endpoint: https://www.affinity.solutions/oauth/revoke
  scopes_supported:
  - mcp
  token_endpoint: https://www.affinity.solutions/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to:
  - https://www.affinity.solutions/wp-json/mcp/mcp-adapter-default-server
  - https://www.affinity.solutions/wp-json/wp-abilities/v1/
  http_scheme: basic
  name: wordpress_application_password
  note: The site's WordPress REST root advertises application-passwords authentication with an authorization endpoint at /wp-admin/authorize-application.php. This gates the wp-abilities/v1 namespace and the second MCP endpoint. It is site-administration auth, not a customer API credential.
  source: https://www.affinity.solutions/wp-json/
  type: http
slug: affinity-solutions-authentication
source_filename: affinity-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://www.affinity.solutions/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the provider's own RFC 8414 authorization-server metadata document and the RFC 9728\n  protected-resource document, both fetched anonymously at HTTP 200. derive-authentication.py produced\n  nothing because the provider publishes no OpenAPI; these fields are read verbatim from the discovery\n  documents, not inferred.\nschemes:\n- name: oauth2_mcp\n  type: oauth2\n  flow: authorization_code\n  pkce:\n    required_methods: [S256]\n  issuer: https://www.affinity.solutions\n  authorization_endpoint: https://www.affinity.solutions/oauth/authorize\n  token_endpoint: https://www.affinity.solutions/oauth/token\n  revocation_endpoint: https://www.affinity.solutions/oauth/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [none]\n  scopes_supported:\
  \ [mcp]\n  client_registration:\n    dynamic_registration_endpoint: null\n    client_id_metadata_document_supported: true\n    note: >-\n      No RFC 7591 dynamic client registration endpoint is advertised. Instead the server declares\n      client_id_metadata_document_supported, so a client identifies itself with a URL-shaped client_id\n      resolving to its own metadata document. Public clients only (token_endpoint_auth_methods_supported\n      is [\"none\"]), which is the OAuth 2.1 public-client-with-PKCE profile MCP expects.\n  applies_to:\n  - https://www.affinity.solutions/wp-json/mcp/mcp-oauth-server\n- name: wordpress_application_password\n  type: http\n  http_scheme: basic\n  source: https://www.affinity.solutions/wp-json/\n  note: >-\n    The site's WordPress REST root advertises application-passwords authentication with an authorization\n    endpoint at /wp-admin/authorize-application.php. This gates the wp-abilities/v1 namespace and the\n    second MCP endpoint. It is site-administration\
  \ auth, not a customer API credential.\n  applies_to:\n  - https://www.affinity.solutions/wp-json/mcp/mcp-adapter-default-server\n  - https://www.affinity.solutions/wp-json/wp-abilities/v1/\nproduct_api_auth:\n  documented: false\n  note: >-\n    No authentication documentation exists for the Comet / Consumer Purchase Insights data products.\n    Access is contracted through clean rooms, a Snowflake Native App and managed services, none of which\n    publish a public credential model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity-solutions/refs/heads/main/authentication/affinity-solutions-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- Analytics
- Consumer Purchase Data
- Transaction Data
- Marketing
- Advertising
- Measurements
- Financial Services
- Retail
- MCP
---
