---
api_key_in: []
api_specs:
- filename: yardi-canada-status-openapi.yml
  format: yaml
  label: Yardi Systems Status API
  slug: yardi-systems-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-status-openapi.yml
auth_types:
- oauth2
- opaque-token
- none
description: ''
kind: authentication
layout: security
method: searched
name: Yardi Canada Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Yardi Canada secures its APIs with oauth2, opaque-token, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Yardi Canada
provider_slug: yardi-canada
scheme_count: 4
schemes:
- applies_to: Yardi Virtuoso Connector (MCP), https://mcp.virtuoso.ai
  authorization_boundary: Scopes carry identity only. Yardi states data access "automatically follows existing user permissions", so the effective authorization is the caller's Yardi role in the tenancy — including a Yardi Canada Ltd. client's Canadian tenancy.
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  documented: true
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.virtuoso.ai/oauth/authorize
      registrationUrl: https://mcp.virtuoso.ai/oauth/register
      scopes:
        email: Email claim
        offline_access: Refresh token issuance
        openid: OpenID Connect identity
        profile: Basic profile claims
      tokenUrl: https://mcp.virtuoso.ai/oauth/token
  machine_readable: true
  name: virtuoso-mcp-oauth
  pkce: required-capable
  sources:
  - well-known/yardi-canada-oauth-protected-resource.json
  - well-known/yardi-canada-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - none
  type: oauth2
- applies_to: RentCafe API (partner-gated)
  detail: The published RentCafe API Terms of Use is the only first-party statement of the credential model. It describes a per-company access token issued under the RentCafe API Access Agreement and its revocation — "The Company's access token will terminate and Company will no longer have access to the Data Exchange Program". No token format, header name, issuance endpoint, expiry, refresh flow, scope vocabulary or rate-limit policy is published anywhere public.
  documented: partially
  issuance: Contract — RentCafe API Access Agreement with Yardi Systems, Inc.
  machine_readable: false
  name: rentcafe-access-token
  source: https://resources.yardi.com/legal/rc-api-tou/
  type: opaque-token
- applies_to: Yardi Voyager Standard Interfaces (partner-gated)
  detail: No credential model is published for the twelve Voyager Standard Interface families. Access is granted only after acceptance into the Interface Partnership Program and execution of a Data Exchange Agreement per interface type.
  documented: false
  name: voyager-interface-credentials
  source: https://www.yardi.com/company/become-an-interface-partner/
  type: unpublished
- applies_to: Yardi Systems Status API, https://status.yardi.com/api/v2
  detail: Public and unauthenticated; every endpoint returns 200 to an anonymous GET.
  documented: true
  name: status-api-anonymous
  source: https://status.yardi.com/api
  type: none
slug: yardi-canada-authentication
source_filename: yardi-canada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://mcp.virtuoso.ai/.well-known/oauth-authorization-server\ndocs:\n  - https://mcp.virtuoso.ai/.well-known/oauth-authorization-server\n  - https://mcp.virtuoso.ai/.well-known/oauth-protected-resource\n  - https://resources.yardi.com/legal/rc-api-tou/\n  - https://status.yardi.com/api\nsummary:\n  types: [oauth2, opaque-token, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  headline: >-\n    Three different authentication regimes coexist and only one of them is documented\n    machine-readably. The Yardi Virtuoso MCP server publishes a full OAuth 2.1\n    authorization-code + PKCE contract anonymously, including dynamic client\n    registration. The Voyager Standard Interfaces and the RentCafe API are governed by\n    signed agreements and an opaque, contract-issued access token with no published\n    header name, format, issuance endpoint or refresh flow. The public status API takes\n    no credential at\
  \ all.\nschemes:\n  - name: virtuoso-mcp-oauth\n    type: oauth2\n    applies_to: Yardi Virtuoso Connector (MCP), https://mcp.virtuoso.ai\n    documented: true\n    machine_readable: true\n    flows:\n      authorizationCode:\n        authorizationUrl: https://mcp.virtuoso.ai/oauth/authorize\n        tokenUrl: https://mcp.virtuoso.ai/oauth/token\n        registrationUrl: https://mcp.virtuoso.ai/oauth/register\n        scopes:\n          openid: OpenID Connect identity\n          profile: Basic profile claims\n          email: Email claim\n          offline_access: Refresh token issuance\n    pkce: required-capable\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, none]\n    bearer_methods_supported: [header]\n    dynamic_client_registration: true\n    authorization_boundary: >-\n      Scopes carry identity only. Yardi states data access \"automatically follows\n      existing user permissions\", so the effective\
  \ authorization is the caller's Yardi\n      role in the tenancy — including a Yardi Canada Ltd. client's Canadian tenancy.\n    sources:\n      - well-known/yardi-canada-oauth-protected-resource.json\n      - well-known/yardi-canada-oauth-authorization-server.json\n  - name: rentcafe-access-token\n    type: opaque-token\n    applies_to: RentCafe API (partner-gated)\n    documented: partially\n    machine_readable: false\n    detail: >-\n      The published RentCafe API Terms of Use is the only first-party statement of the\n      credential model. It describes a per-company access token issued under the\n      RentCafe API Access Agreement and its revocation — \"The Company's access token\n      will terminate and Company will no longer have access to the Data Exchange\n      Program\". No token format, header name, issuance endpoint, expiry, refresh flow,\n      scope vocabulary or rate-limit policy is published anywhere public.\n    issuance: Contract — RentCafe API Access Agreement\
  \ with Yardi Systems, Inc.\n    source: https://resources.yardi.com/legal/rc-api-tou/\n  - name: voyager-interface-credentials\n    type: unpublished\n    applies_to: Yardi Voyager Standard Interfaces (partner-gated)\n    documented: false\n    detail: >-\n      No credential model is published for the twelve Voyager Standard Interface\n      families. Access is granted only after acceptance into the Interface Partnership\n      Program and execution of a Data Exchange Agreement per interface type.\n    source: https://www.yardi.com/company/become-an-interface-partner/\n  - name: status-api-anonymous\n    type: none\n    applies_to: Yardi Systems Status API, https://status.yardi.com/api/v2\n    documented: true\n    detail: Public and unauthenticated; every endpoint returns 200 to an anonymous GET.\n    source: https://status.yardi.com/api\nfederated_identity:\n  openid_connect_discovery: not published on any Yardi web host\n  probes:\n    - {url: 'https://www.yardi.com/.well-known/openid-configuration',\
  \ status: 404}\n    - {url: 'https://www.yardibreeze.ca/.well-known/openid-configuration', status: 404}\n    - {url: 'https://virtuoso.ai/.well-known/openid-configuration', status: 200, note: SPA HTML shell, not a discovery document}\n  product_sso: >-\n    Yardi's cloud-security page states the products offer \"SSO integration\", password\n    complexity/expiry controls and automated inactivity log-off, but publishes no\n    protocol metadata, no IdP endpoints and no SAML metadata URL.\n  source: https://www.yardi.com/company/cloud-security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/authentication/yardi-canada-authentication.yml
summary_line: oauth2/opaque-token/none · 4 schemes
tags:
- Real-Estate
- Canada
- Property Management
- Rentals
- Commercial Real Estate
- PropTech
- Multifamily
- Affordable Housing
- Senior Living
- Investment Management
- Tenancy
- Payments
- MCP
- Artificial Intelligence
---
