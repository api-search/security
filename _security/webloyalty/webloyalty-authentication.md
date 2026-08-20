---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Webloyalty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Webloyalty declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Webloyalty
provider_slug: webloyalty
scheme_count: 2
schemes:
- bearer_methods:
  - header
  client_id_metadata_document_supported: true
  flows:
    authorization_code:
      authorization_url: https://webloyalty.co.uk/oauth/authorize
      pkce_required_methods:
      - S256
      refresh_supported: true
      scopes:
        mcp: Access the Webloyalty MCP endpoint (only scope the server advertises)
      token_url: https://webloyalty.co.uk/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: mcp-oauth
  in: header
  issuer: https://webloyalty.co.uk
  notes:
  - token_endpoint_auth_methods_supported is ["none"] — public clients only, no client secret. PKCE S256 is the only code-challenge method advertised, which is what MCP's authorization spec requires of public clients.
  - 'client_id_metadata_document_supported: true means clients identify themselves by a URL to a client metadata document rather than pre-registering.'
  - A bare GET of https://webloyalty.co.uk/oauth/authorize returns HTTP 400 (missing parameters), which confirms the endpoint is wired and not a stub.
  response_types_supported:
  - code
  revocation_url: https://webloyalty.co.uk/oauth/revoke
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to: https://webloyalty.co.uk/wp-json/
  id: wordpress-application-passwords
  note: The WordPress REST API index advertises application passwords, authorized at https://webloyalty.co.uk/wp-admin/authorize-application.php. This is the CMS's own admin credential path, not a partner-facing API credential.
  scheme: basic
  type: http
slug: webloyalty-authentication
source_filename: webloyalty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://webloyalty.co.uk/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the RFC 8414 authorization-server metadata Webloyalty serves on\n  webloyalty.co.uk, not from an OpenAPI (none is published) and not from a docs\n  page (there is no developer portal). This authorization server exists to guard\n  one thing: the site's MCP endpoint. Webloyalty's commercial integration\n  (\"bespoke API solutions\" on the what-we-offer page) documents no auth model\n  publicly.\nschemes:\n- id: mcp-oauth\n  type: oauth2\n  in: header\n  bearer_methods:\n  - header\n  issuer: https://webloyalty.co.uk\n  flows:\n    authorization_code:\n      authorization_url: https://webloyalty.co.uk/oauth/authorize\n      token_url: https://webloyalty.co.uk/oauth/token\n      refresh_supported: true\n      pkce_required_methods:\n      - S256\n      scopes:\n        mcp: Access the Webloyalty MCP endpoint (only scope the server advertises)\n\
  \  revocation_url: https://webloyalty.co.uk/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  client_id_metadata_document_supported: true\n  notes:\n  - >-\n    token_endpoint_auth_methods_supported is [\"none\"] — public clients only, no\n    client secret. PKCE S256 is the only code-challenge method advertised, which\n    is what MCP's authorization spec requires of public clients.\n  - >-\n    client_id_metadata_document_supported: true means clients identify themselves\n    by a URL to a client metadata document rather than pre-registering.\n  - >-\n    A bare GET of https://webloyalty.co.uk/oauth/authorize returns HTTP 400\n    (missing parameters), which confirms the endpoint is wired and not a stub.\n- id: wordpress-application-passwords\n  type: http\n  scheme: basic\n  note: >-\n    The WordPress REST API index advertises application passwords, authorized\
  \ at\n    https://webloyalty.co.uk/wp-admin/authorize-application.php. This is the\n    CMS's own admin credential path, not a partner-facing API credential.\n  applies_to: https://webloyalty.co.uk/wp-json/\ndocs: null\ndocs_note: >-\n  No public authentication documentation exists. Searched webloyalty.com,\n  webloyalty.co.uk (all 13 sitemap pages) and the locale sites — no developer\n  portal, no API reference, no auth guide.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webloyalty/refs/heads/main/authentication/webloyalty-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Loyalty
- Rewards
- E-Commerce
- Customer Engagement
- Marketing
- Retail
- Cashback
---
