---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trulioo-verifications-api-openapi.yml
  format: yaml
  label: Trulioo Verifications API
  slug: trulioo-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-verifications-api-openapi.yml
- filename: trulioo-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Configuration API
  slug: trulioo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-configuration-api-openapi.yml
- filename: trulioo-connection-api-openapi.yml
  format: yaml
  label: Trulioo Connection API
  slug: trulioo-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-connection-api-openapi.yml
- filename: trulioo-business-verification-api-openapi.yml
  format: yaml
  label: Trulioo Business Verification API
  slug: trulioo-business-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-verification-api-openapi.yml
- filename: trulioo-person-fraud-api-openapi.yml
  format: yaml
  label: Trulioo Person Fraud API
  slug: trulioo-person-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-person-fraud-api-openapi.yml
- filename: trulioo-document-verification-api-openapi.yml
  format: yaml
  label: Trulioo Identity Document Verification API
  slug: trulioo-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-document-verification-api-openapi.yml
- filename: trulioo-authentication-api-openapi.yml
  format: yaml
  label: Trulioo Authentication API
  slug: trulioo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-authentication-api-openapi.yml
- filename: trulioo-business-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Business Configuration API
  slug: trulioo-business-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-configuration-api-openapi.yml
- filename: trulioo-business-reports-api-openapi.yml
  format: yaml
  label: Trulioo Business Reports API
  slug: trulioo-business-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-reports-api-openapi.yml
- filename: trulioo-business-search-api-openapi.yml
  format: yaml
  label: Trulioo Business Search API
  slug: trulioo-business-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-search-api-openapi.yml
- filename: trulioo-document-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Document Configuration API
  slug: trulioo-document-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-document-configuration-api-openapi.yml
- filename: trulioo-documents-api-openapi.yml
  format: yaml
  label: Trulioo Documents API
  slug: trulioo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-documents-api-openapi.yml
- filename: trulioo-end-clients-api-openapi.yml
  format: yaml
  label: Trulioo End Clients API
  slug: trulioo-end-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-end-clients-api-openapi.yml
- filename: trulioo-events-api-openapi.yml
  format: yaml
  label: Trulioo Events API
  slug: trulioo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-events-api-openapi.yml
- filename: trulioo-flows-api-openapi.yml
  format: yaml
  label: Trulioo Flows API
  slug: trulioo-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-flows-api-openapi.yml
- filename: trulioo-known-faces-api-openapi.yml
  format: yaml
  label: Trulioo Known Faces API
  slug: trulioo-known-faces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-known-faces-api-openapi.yml
- filename: trulioo-sessions-api-openapi.yml
  format: yaml
  label: Trulioo Sessions API
  slug: trulioo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-sessions-api-openapi.yml
- filename: trulioo-transactions-api-openapi.yml
  format: yaml
  label: Trulioo Transactions API
  slug: trulioo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-transactions-api-openapi.yml
- filename: trulioo-workflows-api-openapi.yml
  format: yaml
  label: Trulioo Workflows API
  slug: trulioo-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-workflows-api-openapi.yml
auth_types:
- oauth2
- http
- mutualTLS
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Trulioo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode (MCP, PKCE)
overview: Trulioo secures its APIs with oauth2, http, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode (MCP, PKCE) flow(s).
provider_name: Trulioo
provider_slug: trulioo
scheme_count: 4
schemes:
- credential_issuance: Client Id and Client Secret are provided by the Customer Success Manager; no self-serve key creation
  docs: https://developer.trulioo.com/reference/authentication
  documented_token_endpoints:
  - https://auth-api.trulioo.com/connect/token (grant_type=client_credentials, scope=napi.api; Normalized API v3 / GlobalGateway)
  - https://api.trulioo.com/customer/v2/auth/customer (postAuthCustomer; Trulioo Platform / Workflow Studio, access tokens expire in one hour, refresh endpoint available)
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.trulioo.com/customer/v2/auth/customer
  name: OAuth2
  scopes_documented:
  - napi.api
  - workflow.studio.api (authentication recipe)
  sources:
  - openapi/trulioo-authentication-api-openapi.yml
  - openapi/trulioo-business-configuration-api-openapi.yml
  - openapi/trulioo-business-reports-api-openapi.yml
  - openapi/trulioo-business-search-api-openapi.yml
  - openapi/trulioo-business-verification-api-openapi.yml
  - openapi/trulioo-configuration-api-openapi.yml
  - openapi/trulioo-connection-api-openapi.yml
  - openapi/trulioo-document-configuration-api-openapi.yml
  - openapi/trulioo-document-verification-api-openapi.yml
  - openapi/trulioo-documents-api-openapi.yml
  - openapi/trulioo-end-clients-api-openapi.yml
  - openapi/trulioo-events-api-openapi.yml
  - openapi/trulioo-flows-api-openapi.yml
  - openapi/trulioo-known-faces-api-openapi.yml
  - openapi/trulioo-person-fraud-api-openapi.yml
  - openapi/trulioo-sessions-api-openapi.yml
  - openapi/trulioo-transactions-api-openapi.yml
  - openapi/trulioo-verifications-api-openapi.yml
  - openapi/trulioo-workflows-api-openapi.yml
  type: oauth2
- name: BasicAuth
  note: Declared in the v3 contract as an alternative scheme; the docs describe OAuth bearer tokens as the Platform API V3 method
  scheme: basic
  sources:
  - openapi/trulioo-business-configuration-api-openapi.yml
  - openapi/trulioo-business-reports-api-openapi.yml
  - openapi/trulioo-business-search-api-openapi.yml
  - openapi/trulioo-business-verification-api-openapi.yml
  - openapi/trulioo-configuration-api-openapi.yml
  - openapi/trulioo-connection-api-openapi.yml
  - openapi/trulioo-document-configuration-api-openapi.yml
  - openapi/trulioo-document-verification-api-openapi.yml
  - openapi/trulioo-documents-api-openapi.yml
  - openapi/trulioo-known-faces-api-openapi.yml
  - openapi/trulioo-person-fraud-api-openapi.yml
  - openapi/trulioo-transactions-api-openapi.yml
  - openapi/trulioo-verifications-api-openapi.yml
  type: http
- docs: https://developer.trulioo.com/reference/connecting-to-trulioos-api-using-mutual-tls
  name: MutualTLS
  note: Mutual TLS client-certificate connection option documented for the API, configured with Trulioo support
  sources:
  - https://developer.trulioo.com/reference/connecting-to-trulioos-api-using-mutual-tls.md
  type: mutualTLS
- docs: https://mcp.trulioo.com/developer/#auth
  flows:
  - authorizationUrl: https://mcp.trulioo.com/authorize
    flow: authorizationCode
    note: 'Sandbox sessions: client-managed OAuth 2.1 with dynamic client registration'
    pkce: S256
    registrationUrl: https://mcp.trulioo.com/register
    scopes:
    - read
    - verify
    - verification:create
    - kyb:submit
    - agent:write
    - domain:write
    - release:publish
    - release:revoke
    - sandbox:write
    tokenUrl: https://mcp.trulioo.com/token
  - flow: clientCredentials
    note: 'Live integrations: HTTP Basic client_id:client_secret, grant_type=client_credentials -> bearer, expires_in 3600, no refresh token'
    tokenUrl: https://mcp.trulioo.com/oauth/token
  name: MCP OAuth 2.1
  protected_resource: https://mcp.trulioo.com/.well-known/oauth-protected-resource/mcp
  sources:
  - https://mcp.trulioo.com/developer/index.md
  - https://mcp.trulioo.com/.well-known/oauth-authorization-server
  type: oauth2
slug: trulioo-authentication
source_filename: trulioo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: searched\nsource:\n- openapi/trulioo-authentication-api-openapi.yml, openapi/trulioo-business-configuration-api-openapi.yml, openapi/trulioo-business-reports-api-openapi.yml,\n  openapi/trulioo-business-search-api-openapi.yml, openapi/trulioo-business-verification-api-openapi.yml, openapi/trulioo-configuration-api-openapi.yml,\n  openapi/trulioo-connection-api-openapi.yml, openapi/trulioo-document-configuration-api-openapi.yml, openapi/trulioo-document-verification-api-openapi.yml,\n  openapi/trulioo-documents-api-openapi.yml, openapi/trulioo-end-clients-api-openapi.yml, openapi/trulioo-events-api-openapi.yml\n  ...\n- https://developer.trulioo.com/reference/authentication.md\n- https://developer.trulioo.com/reference/keys-and-authentication-2.md\n- https://developer.trulioo.com/reference/connecting-to-trulioos-api-using-mutual-tls.md\n- https://developer.trulioo.com/reference/hmac.md\n- https://mcp.trulioo.com/developer/index.md\n- https://mcp.trulioo.com/.well-known/oauth-authorization-server\
  \ (probed)\nsummary:\n  types:\n  - oauth2\n  - http\n  - mutualTLS\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode (MCP, PKCE)\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.trulioo.com/customer/v2/auth/customer\n    scopes: 0\n  sources:\n  - openapi/trulioo-authentication-api-openapi.yml\n  - openapi/trulioo-business-configuration-api-openapi.yml\n  - openapi/trulioo-business-reports-api-openapi.yml\n  - openapi/trulioo-business-search-api-openapi.yml\n  - openapi/trulioo-business-verification-api-openapi.yml\n  - openapi/trulioo-configuration-api-openapi.yml\n  - openapi/trulioo-connection-api-openapi.yml\n  - openapi/trulioo-document-configuration-api-openapi.yml\n  - openapi/trulioo-document-verification-api-openapi.yml\n  - openapi/trulioo-documents-api-openapi.yml\n  - openapi/trulioo-end-clients-api-openapi.yml\n  - openapi/trulioo-events-api-openapi.yml\n  - openapi/trulioo-flows-api-openapi.yml\n  -\
  \ openapi/trulioo-known-faces-api-openapi.yml\n  - openapi/trulioo-person-fraud-api-openapi.yml\n  - openapi/trulioo-sessions-api-openapi.yml\n  - openapi/trulioo-transactions-api-openapi.yml\n  - openapi/trulioo-verifications-api-openapi.yml\n  - openapi/trulioo-workflows-api-openapi.yml\n  docs: https://developer.trulioo.com/reference/authentication\n  documented_token_endpoints:\n  - https://auth-api.trulioo.com/connect/token (grant_type=client_credentials, scope=napi.api; Normalized API v3\n    / GlobalGateway)\n  - https://api.trulioo.com/customer/v2/auth/customer (postAuthCustomer; Trulioo Platform / Workflow Studio, access\n    tokens expire in one hour, refresh endpoint available)\n  credential_issuance: Client Id and Client Secret are provided by the Customer Success Manager; no self-serve key\n    creation\n  scopes_documented:\n  - napi.api\n  - workflow.studio.api (authentication recipe)\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/trulioo-business-configuration-api-openapi.yml\n\
  \  - openapi/trulioo-business-reports-api-openapi.yml\n  - openapi/trulioo-business-search-api-openapi.yml\n  - openapi/trulioo-business-verification-api-openapi.yml\n  - openapi/trulioo-configuration-api-openapi.yml\n  - openapi/trulioo-connection-api-openapi.yml\n  - openapi/trulioo-document-configuration-api-openapi.yml\n  - openapi/trulioo-document-verification-api-openapi.yml\n  - openapi/trulioo-documents-api-openapi.yml\n  - openapi/trulioo-known-faces-api-openapi.yml\n  - openapi/trulioo-person-fraud-api-openapi.yml\n  - openapi/trulioo-transactions-api-openapi.yml\n  - openapi/trulioo-verifications-api-openapi.yml\n  note: Declared in the v3 contract as an alternative scheme; the docs describe OAuth bearer tokens as the Platform\n    API V3 method\n- name: MutualTLS\n  type: mutualTLS\n  docs: https://developer.trulioo.com/reference/connecting-to-trulioos-api-using-mutual-tls\n  note: Mutual TLS client-certificate connection option documented for the API, configured with Trulioo\
  \ support\n  sources:\n  - https://developer.trulioo.com/reference/connecting-to-trulioos-api-using-mutual-tls.md\n- name: MCP OAuth 2.1\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://mcp.trulioo.com/authorize\n    tokenUrl: https://mcp.trulioo.com/token\n    registrationUrl: https://mcp.trulioo.com/register\n    scopes:\n    - read\n    - verify\n    - verification:create\n    - kyb:submit\n    - agent:write\n    - domain:write\n    - release:publish\n    - release:revoke\n    - sandbox:write\n    note: 'Sandbox sessions: client-managed OAuth 2.1 with dynamic client registration'\n  - flow: clientCredentials\n    tokenUrl: https://mcp.trulioo.com/oauth/token\n    note: 'Live integrations: HTTP Basic client_id:client_secret, grant_type=client_credentials -> bearer, expires_in\n      3600, no refresh token'\n  protected_resource: https://mcp.trulioo.com/.well-known/oauth-protected-resource/mcp\n  docs: https://mcp.trulioo.com/developer/#auth\n\
  \  sources:\n  - https://mcp.trulioo.com/developer/index.md\n  - https://mcp.trulioo.com/.well-known/oauth-authorization-server\ndocs: https://developer.trulioo.com/reference/authentication\nwebhook_authentication:\n  header: x-trulioo-signature\n  algorithm: HMAC-SHA256, hex\n  docs: https://developer.trulioo.com/reference/hmac\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/authentication/trulioo-authentication.yml
summary_line: oauth2/http/mutualTLS · 4 schemes
tags:
- Identity Verification
- KYC
- KYB
- AML
- Watchlist Screening
- Biometrics
- Document Verification
- Fraud Prevention
- Compliance
- Global Identity
---
