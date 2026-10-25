---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Ivalua Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ivalua declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ivalua
provider_slug: ivalua
scheme_count: 1
schemes:
- applies_to: https://portal.ivalua.com/mcp
  authorization_url: https://portal.ivalua.com/oauth2/authorize
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  grant_types:
  - client_credentials
  - authorization_code
  issuer: https://portal.ivalua.com
  name: Ivalua portal OAuth 2.0
  pkce:
  - S256
  registration_url: https://portal.ivalua.com/oauth2/register
  resource_indicators_supported: true
  revocation_url: https://portal.ivalua.com/oauth2/revoke
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  token_url: https://portal.ivalua.com/oauth2/token
  type: oauth2
slug: ivalua-authentication
source_filename: ivalua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Ivalua authentication\ngenerated: '2026-10-20'\nmethod: probed\nsource: https://portal.ivalua.com/.well-known/oauth-authorization-server\nschemes:\n  - type: oauth2\n    name: Ivalua portal OAuth 2.0\n    applies_to: https://portal.ivalua.com/mcp\n    issuer: https://portal.ivalua.com\n    authorization_url: https://portal.ivalua.com/oauth2/authorize\n    token_url: https://portal.ivalua.com/oauth2/token\n    revocation_url: https://portal.ivalua.com/oauth2/revoke\n    registration_url: https://portal.ivalua.com/oauth2/register\n    grant_types: [client_credentials, authorization_code]\n    token_endpoint_auth_methods: [client_secret_post, none]\n    pkce: [S256]\n    resource_indicators_supported: true\n    client_id_metadata_document_supported: true\n    bearer_methods: [header]\nnote: >-\n  Read from the anonymous authorization-server and protected-resource metadata on\n  portal.ivalua.com. Ivalua's broader REST/EAI APIs are documented only to customers;\n  their auth\
  \ scheme is not publicly stated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ivalua/refs/heads/main/authentication/ivalua-authentication.yml
summary_line: 1 scheme
tags:
- Procurement
- Source-to-Pay
- Supplier Management
- Contract Management
- Sourcing
- Purchase Orders
- Invoices
- Spend Analytics
- ERP Integration
- Enterprise
---
