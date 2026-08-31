---
api_key_in: []
api_specs:
- filename: datarails-health-api-openapi.yml
  format: yaml
  label: Datarails Health API
  slug: datarails-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-health-api-openapi.yml
- filename: datarails-oauth-api-openapi.yml
  format: yaml
  label: Datarails OAUTH API
  slug: datarails-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-oauth-api-openapi.yml
- filename: datarails-ready-api-openapi.yml
  format: yaml
  label: Datarails Ready API
  slug: datarails-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-ready-api-openapi.yml
- filename: datarails-well-known-api-openapi.yml
  format: yaml
  label: Datarails .well Known API
  slug: datarails-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-well-known-api-openapi.yml
auth_types:
- oauth2
- http
description: Datarails runs two unrelated authentication models across two surfaces. The FinanceOS MCP server uses OAuth 2.1 with PKCE and dynamic client registration (discoverable at RFC 8414 / RFC 9728 well-known endpoints). The Data Gateway Service upload endpoint uses HTTP Basic with the base64 of a Datarails user's username:password — a service account that Datarails documents must not have MFA enabled. Human sign-in to the application supports SAML SSO.
kind: authentication
layout: security
method: searched
name: Datarails Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Datarails secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Datarails
provider_slug: datarails
scheme_count: 3
schemes:
- bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://mcp.datarails.com/authorize
    flow: authorizationCode
    refreshUrl: https://mcp.datarails.com/token
    scopes:
      datarails: Access the caller's Datarails FinanceOS data, subject to their in-app permissions.
    tokenUrl: https://mcp.datarails.com/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://mcp.datarails.com/
  name: FinanceOS MCP OAuth 2.1
  notes:
  - Clients register anonymously; ChatGPT setup instructions explicitly say to leave both OAuth Client ID and Client Secret empty.
  - Authorization must complete in a pop-up; Datarails documents that the flow fails inside an iframe.
  - JWT access tokens expire after 5 minutes and are auto-refreshed for aggregation calls.
  - Tokens are held by the MCP client; Datarails states no credentials are stored in the AI client.
  - The openid-configuration document advertises token_endpoint_auth_methods_supported [none] while the oauth-authorization-server document advertises [client_secret_post, client_secret_basic] for the same endpoints. Recorded as published; the two documents disagree.
  registration_endpoint: https://mcp.datarails.com/register
  response_types_supported:
  - code
  revocation_endpoint: https://mcp.datarails.com/revoke
  sources:
  - https://mcp.datarails.com/.well-known/oauth-authorization-server
  - https://mcp.datarails.com/.well-known/openid-configuration
  - https://mcp.datarails.com/.well-known/oauth-protected-resource/mcp
  surface: https://mcp.datarails.com/mcp
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- credential_form: 'Authorization: basic <base64(username:password)>'
  name: Data Gateway Service HTTP Basic
  notes:
  - Credential is a real Datarails user account used as a sync user.
  - Datarails documents that the sync user must NOT have MFA enabled.
  - No API-key, token or client-credential alternative is documented for this endpoint.
  - Per-filebox authorisation is a separate control - the target Filebox must have "Upload via API" enabled and the caller must supply its UUID.
  scheme: basic
  sources:
  - https://support.datarails.com/hc/en-us/articles/14616773038620-Data-Gateway-Service-DGS-API-Documentation
  surface: https://app.datarails.com/api/v1/fileboxes/upload_file
  type: http
  weakness_note: Long-lived reusable password credentials over HTTP Basic, with MFA required to be off for the account, is the weakest link in the published Datarails auth surface. Recorded as documented, not as a recommendation.
- identity_providers:
  - Okta
  - Microsoft Entra ID / Azure AD
  - generic SAML 2.0
  name: Application SSO
  notes:
  - Human interactive sign-in only; not an API credential.
  - Datarails notes that an active IdP session is required before the MCP OAuth flow will complete for SSO orgs.
  sources:
  - https://support.datarails.com/hc/en-us/articles/10378530614300-Set-up-SSO-authentication
  - https://support.datarails.com/hc/en-us/articles/19754261303324-SAML-and-OKTA-SSO-Configuration
  - https://support.datarails.com/hc/en-us/articles/13816977103772-Microsoft-Azure-SSO-Configuration
  surface: https://auth.datarails.com/
  type: saml
slug: datarails-authentication
source_filename: datarails-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://mcp.datarails.com/.well-known/oauth-authorization-server\ndocs:\n  - https://support.datarails.com/hc/en-us/articles/25849710214556-Datarails-FinanceOS-MCP-Server-Technical-Documentation\n  - https://support.datarails.com/hc/en-us/articles/14616773038620-Data-Gateway-Service-DGS-API-Documentation\n  - https://support.datarails.com/hc/en-us/articles/10378530614300-Set-up-SSO-authentication\ndescription: >-\n  Datarails runs two unrelated authentication models across two surfaces. The\n  FinanceOS MCP server uses OAuth 2.1 with PKCE and dynamic client registration\n  (discoverable at RFC 8414 / RFC 9728 well-known endpoints). The Data Gateway\n  Service upload endpoint uses HTTP Basic with the base64 of a Datarails user's\n  username:password — a service account that Datarails documents must not have\n  MFA enabled. Human sign-in to the application supports SAML SSO.\n\nsummary:\n  types: [oauth2, http]\n  http_schemes:\
  \ [basic]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  pkce: [S256]\n  dynamic_client_registration: true\n  sso: [SAML 2.0, Okta, Microsoft Entra ID / Azure AD]\n\nschemes:\n  - name: FinanceOS MCP OAuth 2.1\n    type: oauth2\n    surface: https://mcp.datarails.com/mcp\n    sources:\n      - https://mcp.datarails.com/.well-known/oauth-authorization-server\n      - https://mcp.datarails.com/.well-known/openid-configuration\n      - https://mcp.datarails.com/.well-known/oauth-protected-resource/mcp\n    issuer: https://mcp.datarails.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.datarails.com/authorize\n        tokenUrl: https://mcp.datarails.com/token\n        refreshUrl: https://mcp.datarails.com/token\n        scopes:\n          datarails: Access the caller's Datarails FinanceOS data, subject to their in-app permissions.\n    registration_endpoint: https://mcp.datarails.com/register\n    revocation_endpoint: https://mcp.datarails.com/revoke\n\
  \    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n    bearer_methods_supported: [header]\n    id_token_signing_alg_values_supported: [RS256]\n    notes:\n      - Clients register anonymously; ChatGPT setup instructions explicitly say to leave both OAuth Client ID and Client Secret empty.\n      - Authorization must complete in a pop-up; Datarails documents that the flow fails inside an iframe.\n      - JWT access tokens expire after 5 minutes and are auto-refreshed for aggregation calls.\n      - Tokens are held by the MCP client; Datarails states no credentials are stored in the AI client.\n      - >-\n        The openid-configuration document advertises token_endpoint_auth_methods_supported [none]\n        while the oauth-authorization-server document advertises [client_secret_post,\n        client_secret_basic]\
  \ for the same endpoints. Recorded as published; the two documents disagree.\n\n  - name: Data Gateway Service HTTP Basic\n    type: http\n    scheme: basic\n    surface: https://app.datarails.com/api/v1/fileboxes/upload_file\n    sources:\n      - https://support.datarails.com/hc/en-us/articles/14616773038620-Data-Gateway-Service-DGS-API-Documentation\n    credential_form: 'Authorization: basic <base64(username:password)>'\n    notes:\n      - Credential is a real Datarails user account used as a sync user.\n      - Datarails documents that the sync user must NOT have MFA enabled.\n      - No API-key, token or client-credential alternative is documented for this endpoint.\n      - Per-filebox authorisation is a separate control - the target Filebox must have \"Upload via API\" enabled and the caller must supply its UUID.\n    weakness_note: >-\n      Long-lived reusable password credentials over HTTP Basic, with MFA\n      required to be off for the account, is the weakest link in the\
  \ published\n      Datarails auth surface. Recorded as documented, not as a recommendation.\n\n  - name: Application SSO\n    type: saml\n    surface: https://auth.datarails.com/\n    sources:\n      - https://support.datarails.com/hc/en-us/articles/10378530614300-Set-up-SSO-authentication\n      - https://support.datarails.com/hc/en-us/articles/19754261303324-SAML-and-OKTA-SSO-Configuration\n      - https://support.datarails.com/hc/en-us/articles/13816977103772-Microsoft-Azure-SSO-Configuration\n    identity_providers: [Okta, Microsoft Entra ID / Azure AD, generic SAML 2.0]\n    notes:\n      - Human interactive sign-in only; not an API credential.\n      - Datarails notes that an active IdP session is required before the MCP OAuth flow will complete for SSO orgs.\n\nauthorization:\n  model: >-\n    The MCP server enforces the caller's existing Datarails permissions\n    server-side. Per Datarails, a user sees only the data they are authorised\n    to access in the tenant, and the MCP\
  \ connection is read-only.\n  tenant_entitlement: >-\n    FinanceOS AI / MCP access is a paid feature enabled per tenant and per\n    user. Denied callers get \"Authentication Denied: It seems like you are not\n    permitted to use this tool.\"\n  feature_flags:\n    use_semantic_layer_v2: gates the get_business_metric_* data tools (default deny)\n    mcp_use_llm_sql_tool: gates the sql_query tool\n  see: scopes/datarails-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/authentication/datarails-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Accounting
- Budgeting
- Forecasting
- Business Intelligence
- Reporting
- Data Integration
- MCP
- Artificial Intelligence
- Excel
- Software-as-a-Service
---
