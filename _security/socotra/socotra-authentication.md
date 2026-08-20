---
api_key_in: []
api_specs:
- filename: socotra-auth-api-openapi.yml
  format: yaml
  label: Socotra Auth API
  slug: socotra-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-auth-api-openapi.yml
- filename: socotra-auxdata-api-openapi.yml
  format: yaml
  label: Socotra Auxdata API
  slug: socotra-auxdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-auxdata-api-openapi.yml
- filename: socotra-billing-api-openapi.yml
  format: yaml
  label: Socotra Billing API
  slug: socotra-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-billing-api-openapi.yml
- filename: socotra-business-stats-api-openapi.yml
  format: yaml
  label: Socotra Business Stats API
  slug: socotra-business-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-business-stats-api-openapi.yml
- filename: socotra-claim-api-openapi.yml
  format: yaml
  label: Socotra Claim API
  slug: socotra-claim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-claim-api-openapi.yml
- filename: socotra-compliance-api-openapi.yml
  format: yaml
  label: Socotra Compliance API
  slug: socotra-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-compliance-api-openapi.yml
- filename: socotra-config-api-openapi.yml
  format: yaml
  label: Socotra Config API
  slug: socotra-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-config-api-openapi.yml
- filename: socotra-contact-api-openapi.yml
  format: yaml
  label: Socotra Contact API
  slug: socotra-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-contact-api-openapi.yml
- filename: socotra-document-api-openapi.yml
  format: yaml
  label: Socotra Document API
  slug: socotra-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-document-api-openapi.yml
- filename: socotra-event-api-openapi.yml
  format: yaml
  label: Socotra Event API
  slug: socotra-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-event-api-openapi.yml
- filename: socotra-migration-api-openapi.yml
  format: yaml
  label: Socotra Migration API
  slug: socotra-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-migration-api-openapi.yml
- filename: socotra-payment-execution-api-openapi.yml
  format: yaml
  label: Socotra Payment Execution API
  slug: socotra-payment-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-payment-execution-api-openapi.yml
- filename: socotra-plugin-api-openapi.yml
  format: yaml
  label: Socotra Plugin API
  slug: socotra-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-plugin-api-openapi.yml
- filename: socotra-policy-api-openapi.yml
  format: yaml
  label: Socotra Policy API
  slug: socotra-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-policy-api-openapi.yml
- filename: socotra-producers-api-openapi.yml
  format: yaml
  label: Socotra Producers API
  slug: socotra-producers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-producers-api-openapi.yml
- filename: socotra-resource-api-openapi.yml
  format: yaml
  label: Socotra Resource API
  slug: socotra-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-resource-api-openapi.yml
- filename: socotra-search-api-openapi.yml
  format: yaml
  label: Socotra Search API
  slug: socotra-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-search-api-openapi.yml
- filename: socotra-work-management-api-openapi.yml
  format: yaml
  label: Socotra Work Management API
  slug: socotra-work-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socotra/refs/heads/main/openapi/socotra-work-management-api-openapi.yml
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
- MCP
---
