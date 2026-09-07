---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accountsiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: AccountsIQ declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AccountsIQ
provider_slug: accountsiq
scheme_count: 2
schemes:
- api: accountsiq:integration-2-0
  credential_transport:
    fields:
    - description: The bearer access token returned by TokenGet or TokenRefresh.
      name: AccessToken
    - description: The AccountsIQ entity (client company) the call operates against. Multi-entity is a first-class part of the auth context, not a query parameter — the same credentials address different entities by changing this header. GetEntitiesByToken lists the entities a token can reach.
      name: Entity
    header_type: AiqSoapHeader
    mechanism: soap-header
  description: Integration 2.0 authenticates with an OAuth 2.0 client-credentials exchange carried over SOAP rather than over a REST token endpoint. TokenGet(clientId, clientSecret) returns a TokenGetResponse containing AccessToken and RefreshToken. TokenRefresh(clientId, clientSecret, refreshToken) rotates both.
  expiry:
    description: Responses carry a HasExpired boolean; on true, call TokenRefresh.
    signal: WSResultStatus.HasExpired
  flow: client_credentials
  id: aiq-oauth2-client-credentials
  legacy_parameter:
    note: Every 2.0 operation still takes a token as its first parameter for 1.1 compatibility. The provider documents that it should be left BLANK on 2.0 because the token is carried in the header instead.
  scopes:
    note: No OAuth scope surface is published. Authorization is expressed as AccountsIQ user permissions rather than scopes — the 2.0 WSDL annotates read operations with the documentation string "Read Permission Required." No scopes/ artifact is emitted, because asserting a scope list the provider does not publish would be fabrication.
    published: false
  token_operations:
    obtain: TokenGet
    refresh: TokenRefresh
    response_fields:
    - AccessToken
    - RefreshToken
    response_type: TokenGetResponse
  type: oauth2
- api: accountsiq:integration-1-1
  credential_transport:
    mechanism: operation-parameter
    parameter: token (first argument of every method)
  credentials:
  - description: The AccountsIQ entity / company identifier.
    name: companyID
  - description: Integrator partner key, issued by AccountsIQ. Staging and production keys are different sets; production keys must be requested from AccountsIQ directly.
    name: partnerKey
  - description: End-user integration key, generated inside the customer's AIQ deployment.
    name: userKey
  description: Integration 1.1 authenticates with Login(companyID, partnerKey, userKey), which returns a session token string. The token is passed as the first parameter of every subsequent operation.
  expiry:
    lifetime_minutes: 20
    renewal: Call Login again.
    signal: WSResultStatus.HasExpired
    source: https://accountsiq.github.io/API-Wiki/authentication1.html
  id: aiq-session-login
  type: custom-session-token
slug: accountsiq-authentication
source_filename: accountsiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://accountsiq.github.io/API-Wiki/authentication2.html\ndocs:\n- https://accountsiq.github.io/API-Wiki/authentication2.html\n- https://accountsiq.github.io/API-Wiki/authentication1.html\n- https://accountsiq.github.io/API-Wiki/specifications.html\nnote: >-\n  AccountsIQ publishes two authentication models side by side, one per WSDL contract.\n  Neither is described by an OpenAPI securityScheme — this is a SOAP 1.1 service, so the\n  scheme shapes below were read from the provider's own authentication pages and confirmed\n  against the WSDL (the AiqSoapHeader complexType and the TokenGet/TokenRefresh operations\n  exist in wsdl/accountsiq-integration-2-0.wsdl; Login exists in the 1.1 contract).\n  API access is not self-service: an integrator partner key is issued by AccountsIQ after\n  the API Terms of Use are acknowledged to integration@accountsiq.com, and production keys\n  are separate from staging keys.\nschemes:\n\
  - id: aiq-oauth2-client-credentials\n  api: accountsiq:integration-2-0\n  type: oauth2\n  flow: client_credentials\n  description: >-\n    Integration 2.0 authenticates with an OAuth 2.0 client-credentials exchange carried over\n    SOAP rather than over a REST token endpoint. TokenGet(clientId, clientSecret) returns a\n    TokenGetResponse containing AccessToken and RefreshToken. TokenRefresh(clientId,\n    clientSecret, refreshToken) rotates both.\n  token_operations:\n    obtain: TokenGet\n    refresh: TokenRefresh\n    response_type: TokenGetResponse\n    response_fields:\n    - AccessToken\n    - RefreshToken\n  credential_transport:\n    mechanism: soap-header\n    header_type: AiqSoapHeader\n    fields:\n    - name: AccessToken\n      description: The bearer access token returned by TokenGet or TokenRefresh.\n    - name: Entity\n      description: >-\n        The AccountsIQ entity (client company) the call operates against. Multi-entity is a\n        first-class part of the auth\
  \ context, not a query parameter — the same credentials\n        address different entities by changing this header. GetEntitiesByToken lists the\n        entities a token can reach.\n  legacy_parameter:\n    note: >-\n      Every 2.0 operation still takes a token as its first parameter for 1.1 compatibility.\n      The provider documents that it should be left BLANK on 2.0 because the token is carried\n      in the header instead.\n  expiry:\n    signal: WSResultStatus.HasExpired\n    description: Responses carry a HasExpired boolean; on true, call TokenRefresh.\n  scopes:\n    published: false\n    note: >-\n      No OAuth scope surface is published. Authorization is expressed as AccountsIQ user\n      permissions rather than scopes — the 2.0 WSDL annotates read operations with the\n      documentation string \"Read Permission Required.\" No scopes/ artifact is emitted,\n      because asserting a scope list the provider does not publish would be fabrication.\n- id: aiq-session-login\n\
  \  api: accountsiq:integration-1-1\n  type: custom-session-token\n  description: >-\n    Integration 1.1 authenticates with Login(companyID, partnerKey, userKey), which returns a\n    session token string. The token is passed as the first parameter of every subsequent\n    operation.\n  credentials:\n  - name: companyID\n    description: The AccountsIQ entity / company identifier.\n  - name: partnerKey\n    description: >-\n      Integrator partner key, issued by AccountsIQ. Staging and production keys are different\n      sets; production keys must be requested from AccountsIQ directly.\n  - name: userKey\n    description: End-user integration key, generated inside the customer's AIQ deployment.\n  credential_transport:\n    mechanism: operation-parameter\n    parameter: token (first argument of every method)\n  expiry:\n    lifetime_minutes: 20\n    signal: WSResultStatus.HasExpired\n    renewal: Call Login again.\n    source: https://accountsiq.github.io/API-Wiki/authentication1.html\n\
  regional_endpoints:\n  note: >-\n    The WSDL is identical across regions; only the host differs. A client must let the user\n    pick the region matching their AccountsIQ URL.\n  hosts:\n  - region: eu1\n    base: https://eu1.accountsiq.com/system/dashboard/integration/\n  - region: eu2\n    base: https://eu2.accountsiq.com/system/dashboard/integration/\n  - region: uk1\n    base: https://uk1.accountsiq.com/system/dashboard/integration/\n  - region: us1\n    base: https://us1.accountsiq.com/system/dashboard/integration/\nkey_handling_obligations:\n  source: https://accountsiq.github.io/API-Wiki/authentication1.html\n  statements:\n  - The integrator partner key is sensitive and the integrator is responsible for its use.\n  - Keys must be inaccessible via reverse engineering.\n  - The API Terms of Use must be read and acknowledged to integration@accountsiq.com before use.\n  - API keys may not be shared with, or borrowed from, a third party (API Terms of Use, clause 1.1).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accountsiq/refs/heads/main/authentication/accountsiq-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Accounting
- Financial Management
- Cloud Accounting
- ERP
- Consolidation
- General Ledger
- Business Intelligence
- SOAP
- Ireland
---
