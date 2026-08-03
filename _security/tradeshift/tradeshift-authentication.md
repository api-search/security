---
api_key_in:
- header
api_specs:
- filename: tradeshift-external-api-openapi.yml
  format: yaml
  label: Tradeshift External API
  slug: tradeshift-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-external-api-openapi.yml
- filename: tradeshift-mcp-bridge-openapi.yml
  format: yaml
  label: Tradeshift MCP Server
  slug: tradeshift-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-mcp-bridge-openapi.yml
auth_types:
- oauth1
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tradeshift Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- clientCredentials
overview: Tradeshift secures its APIs with oauth1, oauth2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit and clientCredentials flow(s).
provider_name: Tradeshift
provider_slug: tradeshift
scheme_count: 4
schemes:
- credentials:
  - consumer key
  - consumer secret
  - token
  - token secret
  legs: two-legged
  name: TradeshiftOAuth1
  obtain_via: Activate the "API Access to Own Account" app in the Tradeshift App Store; the app displays the four values.
  signature_method: HMAC-SHA1
  sources:
  - https://developers.tradeshift.com/docs/api
  - https://api.tradeshift.com/
  status: 'Supported for backward compatibility. Tradeshift''s own key-concepts documentation marks OAuth1 as deprecated: "Tradeshift supports OAuth1 (deprecated, backward compatibility only) and OAuth2".'
  type: oauth1
- credentials:
  - OAuth2 Client Id
  - OAuth2 Client Secret
  - OAuth2 Redirect URI
  flows:
  - authorizationUrl: https://go.tradeshift.com/oauth2/authorize
    flow: implicit
    response_types_supported:
    - token
    tokenUrl: https://api.tradeshift.com/tradeshift/auth/token
  issuer: https://api.tradeshift.com/tradeshift/
  jwks_uri: https://api.tradeshift.com/tradeshift/auth/jwks
  legs: three-legged
  name: TradeshiftOAuth2
  obtain_via: Install the Developer App on Tradeshift, create a Vendor Id, then CREATE APP to be issued a Client Id and Client Secret and to configure the redirect URI, permissions and webhooks.
  semantics: The app acts on behalf of the logged-in Tradeshift user; API calls carry that user's permissions.
  sources:
  - https://developers.tradeshift.com/docs/guides/oauth
  - https://api.tradeshift.com/tradeshift/.well-known/oauth-authorization-server
  token_types:
  - Access Token
  - Refresh Token
  - JWT
  type: oauth2
  userinfo_endpoint: https://api.tradeshift.com/tradeshift/auth/userinfo
- applies_to: https://mcp.tradeshift.com/mcp
  flows:
  - flow: clientCredentials
    tokenUrl: https://mcp.tradeshift.com/oauth/token
    token_endpoint_auth_methods_supported:
    - client_secret_post
  name: TradeshiftMCPOAuth2
  scopes:
  - core
  - network
  - documents
  - company
  - bfr
  - askada
  - all
  sources:
  - https://mcp.tradeshift.com/.well-known/oauth-authorization-server
  - https://mcp.tradeshift.com/.well-known/oauth-protected-resource
  type: oauth2
- applies_to: https://mcp.tradeshift.com (MCP HTTP Bridge & Management)
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/tradeshift-mcp-bridge-openapi.yml
  type: apiKey
slug: tradeshift-authentication
source_filename: tradeshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/tradeshift-mcp-bridge-openapi.yml\ndocs: https://developers.tradeshift.com/docs/guides/oauth\nnote: >-\n  The Tradeshift External API OpenAPI (openapi/tradeshift-external-api-openapi.yml) declares NO securitySchemes and\n  NO security requirements — the auth contract lives only in prose, on the API root, in the developer-center guides,\n  and in the RFC 8414 metadata. This profile therefore upgrades the mechanically derived result (which saw only the\n  MCP bridge's X-API-Key scheme) with what Tradeshift actually documents.\nsummary:\n  types: [oauth1, oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [implicit, clientCredentials]\n  required_headers: [X-Tradeshift-TenantId]\nschemes:\n  - name: TradeshiftOAuth1\n    type: oauth1\n    signature_method: HMAC-SHA1\n    legs: two-legged\n    credentials:\n      - consumer key\n      - consumer secret\n      - token\n      - token secret\n    obtain_via: >-\n   \
  \   Activate the \"API Access to Own Account\" app in the Tradeshift App Store; the app displays the four values.\n    status: >-\n      Supported for backward compatibility. Tradeshift's own key-concepts documentation marks OAuth1 as deprecated:\n      \"Tradeshift supports OAuth1 (deprecated, backward compatibility only) and OAuth2\".\n    sources:\n      - https://developers.tradeshift.com/docs/api\n      - https://api.tradeshift.com/\n  - name: TradeshiftOAuth2\n    type: oauth2\n    legs: three-legged\n    flows:\n      - flow: implicit\n        authorizationUrl: https://go.tradeshift.com/oauth2/authorize\n        tokenUrl: https://api.tradeshift.com/tradeshift/auth/token\n        response_types_supported: [token]\n    jwks_uri: https://api.tradeshift.com/tradeshift/auth/jwks\n    userinfo_endpoint: https://api.tradeshift.com/tradeshift/auth/userinfo\n    issuer: https://api.tradeshift.com/tradeshift/\n    credentials:\n      - OAuth2 Client Id\n      - OAuth2 Client Secret\n    \
  \  - OAuth2 Redirect URI\n    obtain_via: >-\n      Install the Developer App on Tradeshift, create a Vendor Id, then CREATE APP to be issued a Client Id and\n      Client Secret and to configure the redirect URI, permissions and webhooks.\n    token_types: [Access Token, Refresh Token, JWT]\n    semantics: >-\n      The app acts on behalf of the logged-in Tradeshift user; API calls carry that user's permissions.\n    sources:\n      - https://developers.tradeshift.com/docs/guides/oauth\n      - https://api.tradeshift.com/tradeshift/.well-known/oauth-authorization-server\n  - name: TradeshiftMCPOAuth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://mcp.tradeshift.com/oauth/token\n        token_endpoint_auth_methods_supported: [client_secret_post]\n    scopes: [core, network, documents, company, bfr, askada, all]\n    applies_to: https://mcp.tradeshift.com/mcp\n    sources:\n      - https://mcp.tradeshift.com/.well-known/oauth-authorization-server\n\
  \      - https://mcp.tradeshift.com/.well-known/oauth-protected-resource\n  - name: APIKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    applies_to: https://mcp.tradeshift.com (MCP HTTP Bridge & Management)\n    sources:\n      - openapi/tradeshift-mcp-bridge-openapi.yml\ntenancy:\n  header: X-Tradeshift-TenantId\n  required: true\n  value: The UUID of the Tradeshift company account (tenant) being accessed.\n  quote: >-\n    \"All OAuth requests MUST also include a X-Tradeshift-TenantId header, containing the TenantId (a UUID) to be\n    accessed.\" — https://api.tradeshift.com/\n  additional_headers_seen_in_spec:\n    - X-Tradeshift-ActorId\n    - X-Tradeshift-SecurityGroup\nverification:\n  smoke_test: GET https://api-sandbox.tradeshift.com/tradeshift/rest/external/account/info\n  expected: Information about your own company account.\n  source: https://developers.tradeshift.com/docs/api\nx-evidence:\n  - url: https://api.tradeshift.com/\n    http_status: 200\n\
  \    fetched: '2026-08-02'\n  - url: https://api.tradeshift.com/tradeshift/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-02'\n  - url: https://developers.tradeshift.com/rest/docs/api\n    http_status: 200\n    fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/authentication/tradeshift-authentication.yml
summary_line: oauth1/oauth2/apiKey · 4 schemes
tags:
- e-invoicing
- accounts-payable
- ap-automation
- procure-to-pay
- supply-chain
- b2b-commerce
- invoicing
- ubl
- peppol
- e-invoicing-compliance
- supplier-network
- business-documents
- fintech
- mcp
- agent-native
---
