---
api_key_in: []
api_specs:
- filename: socotra-openapi-original.json
  format: json
  label: Socotra Insurance Suite API
  slug: socotra-insurance-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-openapi-original.json
auth_types:
- http
- oauth2
- openIdConnect
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Socotra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Socotra secures its APIs with http, oauth2, openIdConnect, and saml across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Socotra
provider_slug: socotra
scheme_count: 3
schemes:
- description: Socotra Insurance Suite API calls are authenticated with a bearer access token sent in the Authorization header. Tokens are minted from the auth service (POST /auth/users/tokens - createAuthToken) using business-account credentials (business_account_name + username + password), and revoked via revokeUserOauthTokens. Service accounts obtain non-interactive tokens via createServiceAccountAuthToken.
  name: BearerAuth
  scheme: bearer
  sources:
  - documentation
  - npm:@socotra/auth
  type: http
- description: OAuth 2.1 authorization-code flow is used for interactive agent/UI access (e.g. the hosted MCP server at https://mcp-sandbox.socotra.com/mcp redirects to a browser login with business-account credentials).
  flows:
    authorizationCode: {}
  name: OAuth2
  sources:
  - documentation
  type: oauth2
- description: Tenants can federate identity through SAML 2.0 and OIDC identity providers (addSAMLIdentityProvider, addOIDCIdentityProvider) for workforce SSO into the platform. A role/permission model (roles, token permissions, data-access masks) governs authorization.
  name: EnterpriseSSO
  sources:
  - documentation
  - openapi/socotra-openapi-original.json
  type: openIdConnect
slug: socotra-authentication
source_filename: socotra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.socotra.com/\ndocs: https://docs.socotra.com/getting-started/log-into-socotra\nsummary:\n  types: [http, oauth2, openIdConnect, saml]\n  api_key_in: []\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    The published OpenAPI definition does not declare components.securitySchemes;\n    this profile is derived from the Socotra documentation and the @socotra/auth\n    library rather than the spec.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Socotra Insurance Suite API calls are authenticated with a bearer access token\n    sent in the Authorization header. Tokens are minted from the auth service\n    (POST /auth/users/tokens - createAuthToken) using business-account credentials\n    (business_account_name + username + password), and revoked via\n    revokeUserOauthTokens. Service accounts obtain non-interactive tokens via\n    createServiceAccountAuthToken.\n\
  \  sources: [documentation, 'npm:@socotra/auth']\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow is used for interactive agent/UI access\n    (e.g. the hosted MCP server at https://mcp-sandbox.socotra.com/mcp redirects to\n    a browser login with business-account credentials).\n  flows:\n    authorizationCode: {}\n  sources: [documentation]\n- name: EnterpriseSSO\n  type: openIdConnect\n  description: >-\n    Tenants can federate identity through SAML 2.0 and OIDC identity providers\n    (addSAMLIdentityProvider, addOIDCIdentityProvider) for workforce SSO into the\n    platform. A role/permission model (roles, token permissions, data-access masks)\n    governs authorization.\n  sources: [documentation, 'openapi/socotra-openapi-original.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/authentication/socotra-authentication.yml
summary_line: http/oauth2/openIdConnect/saml · 3 schemes
tags:
- Company
- Insurtech
- Insurance
- Core Platform
- Policy Administration
- Billing
- Claims
- Underwriting
- API
- MCP
---
