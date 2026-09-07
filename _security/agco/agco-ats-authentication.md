---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agco-locations-api-openapi.yml
  format: yaml
  label: agco Locations API
  slug: agco-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-locations-api-openapi.yml
- filename: agco-machines-api-openapi.yml
  format: yaml
  label: agco Machines API
  slug: agco-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-machines-api-openapi.yml
- filename: agco-telemetry-api-openapi.yml
  format: yaml
  label: agco Telemetry API
  slug: agco-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-telemetry-api-openapi.yml
- filename: agco-ats-api-openapi.json
  format: json
  label: AGCO ATS API
  slug: agco-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-ats-api-openapi.json
auth_types: []
description: 'The AGCO ATS contract declares NO securityDefinitions — an OpenAPI-level gap, not an open API. In practice the surface is authenticated two ways, both discoverable from the API''s own Authentication resource and the public login page: a first-party username/password login that mints API tokens, and an OpenID Connect flow delegated to an external identity provider. Credentials are issued through the AGCO EDT Support Portal; there is no self-service signup.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Agco Ats Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agco declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Agco
provider_slug: agco
scheme_count: 0
schemes: []
slug: agco-ats-authentication
source_filename: agco-ats-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  openapi/agco-ats-api-openapi.json (live contract, https://secure.agco-ats.com/swagger/docs/v1,\n  fetched 2026-09-04) plus the public sign-in page at https://www.agco-ats.com/login.aspx, which\n  states the credential authority and the OIDC redirect entry point verbatim.\napi: agco:agco-ats-api\ndescription: >-\n  The AGCO ATS contract declares NO securityDefinitions — an OpenAPI-level gap, not an open API. In\n  practice the surface is authenticated two ways, both discoverable from the API's own Authentication\n  resource and the public login page: a first-party username/password login that mints API tokens,\n  and an OpenID Connect flow delegated to an external identity provider. Credentials are issued\n  through the AGCO EDT Support Portal; there is no self-service signup.\nsummary:\n  declared_security_schemes: 0\n  observed_mechanisms: 2\n  self_service: false\n  credential_authority: AGCO EDT Support Portal (EDT_Support@agcocorp.com)\n\
  gaps:\n  - >-\n    securityDefinitions is null and no operation carries a `security` block, so a generated client\n    from this spec sends no credentials at all. Every one of the 285 operations is undocumented as\n    to which mechanism and which permission it requires.\n  - >-\n    The OIDC provider, its issuer URL, its scopes and its discovery document are not published.\n    /.well-known/openid-configuration returns 404 on secure.agco-ats.com (probed 2026-09-04).\nmechanisms:\n  - name: Password login with API tokens\n    type: http\n    scheme: custom\n    flow: >-\n      POST /api/v2/Authentication authenticates a user (operationId Authentication_Default);\n      PUT /api/v2/AuthenticatedUsers/{UserID}/Tokens manages that user's API tokens\n      (operationId Authentication_PutManageTokens).\n    operations:\n      - Authentication_Default\n      - Authentication_PutManageTokens\n      - Authentication_RequestPasswordReset\n      - Authentication_ResetPasword\n    note: >-\n    \
  \  Token transport (header name, prefix, lifetime) is not described in the contract and is not\n      published. Determining it requires credentialed access we do not have and did not attempt.\n  - name: OpenID Connect (delegated)\n    type: openIdConnect\n    flow: authorization_code\n    operations:\n      - Authentication_OAuthRedirect\n      - Authentication_OAuthCallback\n      - Authentication_OAuthUser\n      - Authentication_OAuthCertificate\n    entry_point: https://secure.agco-ats.com/api/v2/Authentication/OAuthRedirect?redirectUri={redirectUri}\n    evidence: >-\n      https://www.agco-ats.com/login.aspx ships a navigateToSSO() function that redirects the browser\n      to /api/v2/Authentication/OAuthRedirect with the current page as redirectUri.\n    detail: >-\n      Authentication_OAuthRedirect redirects to the configured OIDC provider;\n      Authentication_OAuthCallback receives the redirect; Authentication_OAuthUser exchanges the\n      result for an ATS session; Authentication_OAuthCertificate\
  \ returns the certificate used for\n      OAuth client authentication.\n    issuer: null\n    scopes_published: false\nauthorization:\n  model: >-\n    Role- and permission-based, exposed as first-class resources rather than OAuth scopes:\n    /api/v2/Roles, /api/v2/Permissions, /api/v2/UserPermissions, /api/v2/AuthorizationCategories,\n    /api/v2/AuthorizationCodeDefinitions and /api/v2/AuthorizationCodes. Visibility of package types,\n    update groups and authorization categories is granted per user.\n  scopes: []\nhealth_check:\n  operation: Authentication_IsAlive\n  path: /api/v2/Authentication/IsAlive\n  note: Unauthenticated liveness acknowledgement declared in the contract.\nonboarding:\n  self_service: false\n  contact: EDT_Support@agcocorp.com\n  docs: https://www.agco-ats.com/\n  note: >-\n    \"This site now uses login credentials from the EDT Support Portal. For access, please contact\n    EDT_Support@agcocorp.com\" — quoted verbatim from https://www.agco-ats.com/login.aspx,\
  \ 2026-09-04.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/authentication/agco-ats-authentication.yml
summary_line: 0 schemes
tags:
- Fortune 500
- Agriculture
- Farm Equipment
- Manufacturing
- Telematics
- Precision Agriculture
- Diagnostics
---
