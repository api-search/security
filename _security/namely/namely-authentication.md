---
api_key_in: []
api_specs:
- filename: namely-api-openapi.json
  format: json
  label: Namely API
  slug: namely-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-api-openapi.json
auth_types: []
description: 'The Namely API supports two authentication models, both documented on the provider''s own developer portal: a 3-legged OAuth 2.0 authorization code grant for partner integrations, and Personal Access Tokens (bearer tokens) for a client''s own internal integrations. All requests must be made over HTTPS; plaintext HTTP is refused. Credentials are minted inside the customer''s own Namely HRIS tenant under the API menu item, which requires an administrator to grant access.'
kind: authentication
layout: security
method: searched
name: Namely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Namely declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Namely
provider_slug: namely
scheme_count: 3
schemes:
- from_spec: true
  id: Authorization
  in: header
  name: Authorization
  note: The only securityDefinition the published Swagger 2.0 document declares. It is a header credential named Authorization, carrying either an OAuth 2.0 access token or a Personal Access Token as a Bearer value. The spec declares no top-level or per-operation `security` block, so the scheme is defined but never applied inside the contract itself - the docs, not the spec, are what tell an integrator to send it.
  spec_location: securityDefinitions.Authorization
  type: apiKey
- access_token_lifetime: 15 minutes
  authorization_url: https://{company}.namely.com/api/v1/oauth2/authorize
  flow: accessCode
  from_spec: false
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2_authorization_code
  parameters:
  - response_type
  - client_id
  - redirect_uri
  - client_secret
  - code
  - grant_type
  - refresh_token
  refresh_token_lifetime: No stated expiration. The same refresh token is returned on each refresh; Namely's docs warn that clients should always persist the returned refresh token because the lifespan is subject to change.
  registration: Self-service inside the Namely HRIS tenant (API menu -> OAuth Applications). Requires name, website and one or more comma-separated redirect URIs; returns a client identifier and client secret.
  scopes_documented: false
  scopes_note: Namely documents no OAuth scope vocabulary. Authorization is inherited from the Namely user who approves the application, not requested per-scope, so scopes/ is not emitted.
  source: https://developers.namely.com/docs/getting-started/authentication.md
  templated_host: true
  templated_note: Namely is multi-tenant on {company}.namely.com; the authorization and token endpoints live inside each customer's own tenant, not on a shared authorization server.
  token_url: https://{company}.namely.com/api/v1/oauth2/token
  type: oauth2
- failure_mode: If the profile that created a PAT becomes inactive or is deleted, the API returns HTTP 403 to every request using that token and the integration breaks.
  from_spec: false
  header: 'Authorization: Bearer <token>'
  id: personal_access_token
  intended_for: A Namely client building their own custom integration.
  lifetime: 2 years
  not_intended_for: Partner integrations. Namely's docs explicitly say partners should use an OAuth application instead of a PAT.
  permission_model: A PAT carries exactly the permissions of the Namely user who created it. Namely recommends creating integration PATs under a dedicated administrator "Integrations User" profile that persists through staff turnover.
  scheme: bearer
  source: https://developers.namely.com/docs/getting-started/authentication.md
  type: http
slug: namely-authentication
source_filename: namely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developers.namely.com/docs/getting-started/authentication.md\ndocs: https://developers.namely.com/docs/getting-started/authentication.md\nspec: openapi/namely-api-openapi.json\nname: Namely API authentication\ndescription: >-\n  The Namely API supports two authentication models, both documented on the provider's own\n  developer portal: a 3-legged OAuth 2.0 authorization code grant for partner integrations, and\n  Personal Access Tokens (bearer tokens) for a client's own internal integrations. All requests\n  must be made over HTTPS; plaintext HTTP is refused. Credentials are minted inside the customer's\n  own Namely HRIS tenant under the API menu item, which requires an administrator to grant access.\ntransport:\n  https_required: true\n  http_refused: true\n  source: https://developers.namely.com/docs/getting-started/authentication.md\nschemes:\n  - id: Authorization\n    type: apiKey\n    in: header\n    name: Authorization\n\
  \    from_spec: true\n    spec_location: securityDefinitions.Authorization\n    note: >-\n      The only securityDefinition the published Swagger 2.0 document declares. It is a header\n      credential named Authorization, carrying either an OAuth 2.0 access token or a Personal\n      Access Token as a Bearer value. The spec declares no top-level or per-operation `security`\n      block, so the scheme is defined but never applied inside the contract itself - the docs, not\n      the spec, are what tell an integrator to send it.\n  - id: oauth2_authorization_code\n    type: oauth2\n    flow: accessCode\n    from_spec: false\n    source: https://developers.namely.com/docs/getting-started/authentication.md\n    authorization_url: https://{company}.namely.com/api/v1/oauth2/authorize\n    token_url: https://{company}.namely.com/api/v1/oauth2/token\n    grant_types:\n      - authorization_code\n      - refresh_token\n    templated_host: true\n    templated_note: >-\n      Namely is multi-tenant\
  \ on {company}.namely.com; the authorization and token endpoints live\n      inside each customer's own tenant, not on a shared authorization server.\n    parameters:\n      - response_type\n      - client_id\n      - redirect_uri\n      - client_secret\n      - code\n      - grant_type\n      - refresh_token\n    access_token_lifetime: 15 minutes\n    refresh_token_lifetime: >-\n      No stated expiration. The same refresh token is returned on each refresh; Namely's docs warn\n      that clients should always persist the returned refresh token because the lifespan is\n      subject to change.\n    scopes_documented: false\n    scopes_note: >-\n      Namely documents no OAuth scope vocabulary. Authorization is inherited from the Namely user\n      who approves the application, not requested per-scope, so scopes/ is not emitted.\n    registration: >-\n      Self-service inside the Namely HRIS tenant (API menu -> OAuth Applications). Requires name,\n      website and one or more comma-separated\
  \ redirect URIs; returns a client identifier and\n      client secret.\n  - id: personal_access_token\n    type: http\n    scheme: bearer\n    from_spec: false\n    source: https://developers.namely.com/docs/getting-started/authentication.md\n    header: 'Authorization: Bearer <token>'\n    lifetime: 2 years\n    permission_model: >-\n      A PAT carries exactly the permissions of the Namely user who created it. Namely recommends\n      creating integration PATs under a dedicated administrator \"Integrations User\" profile that\n      persists through staff turnover.\n    failure_mode: >-\n      If the profile that created a PAT becomes inactive or is deleted, the API returns HTTP 403\n      to every request using that token and the integration breaks.\n    intended_for: A Namely client building their own custom integration.\n    not_intended_for: >-\n      Partner integrations. Namely's docs explicitly say partners should use an OAuth application\n      instead of a PAT.\nidentity_federation:\n\
  \  saml:\n    supported: true\n    version: SAML 2.0\n    role: Service Provider only\n    source: https://developers.namely.com/docs/getting-started/sso.md\n    note: >-\n      Namely performs no credential authentication of its own for SSO. It verifies the assertion\n      from the customer's Identity Provider and matches the NameID email against an existing\n      Namely profile. Namely publishes a SAML metadata endpoint for IdP configuration. Named\n      supported IdPs are Okta, OneLogin and Microsoft Entra ID (Azure AD).\n    provisioning: >-\n      Namely does NOT provision accounts into the IdP. Inbound/outbound user provisioning is\n      handled separately through the SCIM 2.0 surface (see conformance/namely-conformance.yml).\n  scim:\n    supported: true\n    version: SCIM 2.0\n    endpoint: https://{company}.namely.com/api/scim/v2/Users.json\n    source: https://developers.namely.com/docs/okta/syncing-custom-fields.md\n    note: >-\n      Namely acts as the SCIM source of record\
  \ for user profiles flowing into Okta. Custom\n      attributes are carried under the standard SCIM extension URN\n      urn:ietf:params:scim:schemas:extension:custom:2.0:User.\ngaps:\n  - >-\n    The published Swagger 2.0 document declares no `security` requirement on any of its 54\n    operations, so a generated client will not attach the Authorization header without the\n    integrator reading the prose docs.\n  - >-\n    The OAuth 2.0 flow is documented only in prose. It is absent from the machine-readable\n    contract, which declares apiKey only.\n  - No published OAuth scope vocabulary; consent is all-or-nothing at the user's permission level.\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/authentication/namely-authentication.yml
summary_line: 3 schemes
tags:
- HR
- Human Capital Management
- Payroll
- Employee Data
- Onboarding
- Benefits
- Applicant Tracking
- Performance Management
- SCIM
- Single Sign-On
- Identity Provisioning
- Workforce Management
---
