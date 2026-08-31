---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Granica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Granica declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Granica
provider_slug: granica
scheme_count: 3
schemes:
- default_when_unscoped: If no access policy is selected at creation the key is granted full access to all API endpoints.
  description: Long-lived bearer API key for machine-to-machine access to the Granica REST API without a user session. Keys are created under Settings > API Keys in the Granica Console and are Admin-role only. The full key value is displayed exactly once at creation and cannot be retrieved afterwards.
  expiration:
    behavior: Keys become inactive after their expiration date and can no longer authenticate requests.
    configurable: true
    never_expires_allowed: true
    range_days:
      max: 365
      min: 1
  format: 'Authorization: Bearer <your-api-key>'
  header: Authorization
  id: api_key_bearer
  in: header
  scheme: bearer
  scoped: true
  scopes_artifact: scopes/granica-scopes.yml
  type: http
- applies_to: Granica Console (human users), not the M2M API
  description: Single Sign-On via OpenID Connect. Granica acts as a confidential OIDC client using the Authorization Code flow; configuration requires a discovery URL (.well-known/openid-configuration), client ID and client secret.
  id: console_session_oidc
  identity_providers:
  - Okta
  - Microsoft Entra ID
  - Google Workspace
  - Auth0
  - AWS IAM Identity Center
  - Keycloak
  - Any OpenID Connect Core 1.0 compliant provider
  type: openIdConnect
- applies_to: Granica Console (human users), not the M2M API
  break_glass: Designated break-glass users can always log in with local credentials even when SSO is enforced or the IdP is unavailable. Configured under Settings > SSO before enforcement.
  description: SAML 2.0 SSO with Granica acting as the Service Provider. Configuration imports IdP metadata by URL or XML and registers Granica's SP metadata (Entity ID, ACS URL, SLO URL, SP certificate) with the IdP. Granica signs outbound requests by default.
  enforcement_modes:
  - disabled
  - test
  - enforced
  id: console_session_saml
  identity_providers:
  - Okta
  - Microsoft Entra ID
  - Google Workspace (assertion encryption not supported)
  - Auth0
  - AWS IAM Identity Center (users must be pre-provisioned; SCIM auto-provisioning not supported)
  - Any SAML 2.0 compliant provider
  type: saml2
slug: granica-authentication
source_filename: granica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://docs.granica.ai/security-and-compliance/api-token\ndocs:\n- https://docs.granica.ai/security-and-compliance/api-token\n- https://docs.granica.ai/security-and-compliance/sso-integration\n- https://docs.granica.ai/security-and-compliance/role-based-access-control\n- https://docs.granica.ai/administration/use-platform-tools\nnote: >-\n  Derived from the published docs rather than a securityScheme block - Granica does not publish an OpenAPI\n  file on a public host (the FastAPI /openapi.json is served only from the customer's own deployed Granica\n  Console, admin-only, at /granica-api/openapi.json).\napi: Granica APIs V1\nbase_path: /api/v1\nschemes:\n- id: api_key_bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <your-api-key>'\n  description: >-\n    Long-lived bearer API key for machine-to-machine access to the Granica REST API without a user session.\n\
  \    Keys are created under Settings > API Keys in the Granica Console and are Admin-role only. The full key\n    value is displayed exactly once at creation and cannot be retrieved afterwards.\n  scoped: true\n  scopes_artifact: scopes/granica-scopes.yml\n  expiration:\n    configurable: true\n    range_days:\n      min: 1\n      max: 365\n    never_expires_allowed: true\n    behavior: Keys become inactive after their expiration date and can no longer authenticate requests.\n  default_when_unscoped: >-\n    If no access policy is selected at creation the key is granted full access to all API endpoints.\n- id: console_session_oidc\n  type: openIdConnect\n  applies_to: Granica Console (human users), not the M2M API\n  description: >-\n    Single Sign-On via OpenID Connect. Granica acts as a confidential OIDC client using the Authorization\n    Code flow; configuration requires a discovery URL (.well-known/openid-configuration), client ID and\n    client secret.\n  identity_providers:\n\
  \  - Okta\n  - Microsoft Entra ID\n  - Google Workspace\n  - Auth0\n  - AWS IAM Identity Center\n  - Keycloak\n  - Any OpenID Connect Core 1.0 compliant provider\n- id: console_session_saml\n  type: saml2\n  applies_to: Granica Console (human users), not the M2M API\n  description: >-\n    SAML 2.0 SSO with Granica acting as the Service Provider. Configuration imports IdP metadata by URL or\n    XML and registers Granica's SP metadata (Entity ID, ACS URL, SLO URL, SP certificate) with the IdP.\n    Granica signs outbound requests by default.\n  identity_providers:\n  - Okta\n  - Microsoft Entra ID\n  - Google Workspace (assertion encryption not supported)\n  - Auth0\n  - AWS IAM Identity Center (users must be pre-provisioned; SCIM auto-provisioning not supported)\n  - Any SAML 2.0 compliant provider\n  enforcement_modes:\n  - disabled\n  - test\n  - enforced\n  break_glass: >-\n    Designated break-glass users can always log in with local credentials even when SSO is enforced or the\n\
  \    IdP is unavailable. Configured under Settings > SSO before enforcement.\nsessions:\n  token_type: JWT\n  access_token_ttl_seconds:\n    default: 3600\n    range: [900, 28800]\n  refresh_token_ttl_seconds:\n    sso_users_default: 7200\n    range: [3600, 28800]\n  propagation: Changes apply to newly issued tokens within 60 seconds.\n  source: https://docs.granica.ai/administration/configure-crunch\nrbac:\n  roles:\n  - Admin\n  - Editor\n  - Viewer\n  enforcement:\n  - GET (read) requests are available to all authenticated users.\n  - POST, PUT, PATCH and DELETE (write) requests are restricted to Editors and Admins.\n  - The /docs, /redoc and /openapi.json API documentation UI is Admin-only.\n  - API-key scopes are enforced in addition to role - a key with only tables:read cannot trigger a crunch job.\n  source: https://docs.granica.ai/security-and-compliance/role-based-access-control\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granica/refs/heads/main/authentication/granica-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Data
- Storage
- Analytics
- Artificial Intelligence
- Machine-Learning
- Data Lakehouse
- Cloud Cost Optimization
- Compression
- Data Infrastructure
---
