---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Xage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xage declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Xage
provider_slug: xage
scheme_count: 1
schemes:
- applies_to: https://xage.com/wp-json/mcp/mcp-oauth-server
  authorization_response_iss_parameter_supported: true
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  dynamic_client_registration: false
  evidence:
  - status: 200
    url: https://xage.com/.well-known/oauth-authorization-server
  - status: 200
    url: https://xage.com/.well-known/oauth-protected-resource
  - status: 401
    url: https://xage.com/wp-json/mcp/mcp-oauth-server
  flows:
    authorization_code:
      authorization_url: https://xage.com/oauth/authorize
      refresh_url: https://xage.com/oauth/token
      revocation_url: https://xage.com/oauth/revoke
      scopes:
        mcp: Access the Model Context Protocol server
      token_url: https://xage.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp_oauth2
  pkce_required_methods:
  - S256
  public_client: true
  response_types:
  - code
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: xage-authentication
source_filename: xage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://xage.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the two OAuth discovery documents Xage actually serves on xage.com. These describe\n  authentication to the WordPress-hosted MCP server on the marketing site, NOT to the Xage Fabric\n  Platform product API — see mcp/xage-mcp.yml. The Fabric Manager API's own auth model is not\n  publicly documented; the only public third-party description (Axonius' Xage adapter) states it\n  accepts either a username/password credential or an access-request token bound to a user account,\n  against a customer-supplied Xage server hostname or IP.\nschemes:\n- id: mcp_oauth2\n  type: oauth2\n  applies_to: https://xage.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorization_code:\n      authorization_url: https://xage.com/oauth/authorize\n      token_url: https://xage.com/oauth/token\n      refresh_url: https://xage.com/oauth/token\n      revocation_url: https://xage.com/oauth/revoke\n\
  \      scopes:\n        mcp: Access the Model Context Protocol server\n  pkce_required_methods: [S256]\n  response_types: [code]\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  bearer_methods: [header]\n  public_client: true\n  dynamic_client_registration: false\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\n  evidence:\n  - url: https://xage.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://xage.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://xage.com/wp-json/mcp/mcp-oauth-server\n    status: 401\nundocumented_surfaces:\n- name: Xage Fabric Manager REST API\n  reason: >-\n    Reference is published only inside the customer-authenticated Xage support portal\n    (xage.zendesk.com / support.xage.com). The Zendesk Help Center API returns\n    401 \"Couldn't authenticate you\" anonymously, so no auth documentation could be read.\n \
  \ evidence:\n  - url: https://xage.zendesk.com/api/v2/help_center/en-us/articles.json\n    status: 401\n  - url: https://xage.com/support/\n    status: 200\n  third_party_description:\n    source: https://docs.axonius.com/docs/xage\n    methods: [username-password, access-request-token]\n    host: customer-supplied Xage server hostname or IP address\ndocs: null\ndocs_note: Xage publishes no public authentication documentation page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xage/refs/heads/main/authentication/xage-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Zero Trust
- Identity and Access Management
- Privileged Access Management
- Operational Technology
- Critical Infrastructure
- Industrial
- Agent Security
---
