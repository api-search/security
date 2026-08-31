---
api_key_in: []
api_specs:
- filename: metabolon-assistant-api-openapi.yml
  format: yaml
  label: Metabolon Assistant API
  slug: metabolon-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-assistant-api-openapi.yml
- filename: metabolon-auth-api-openapi.yml
  format: yaml
  label: Metabolon Auth API
  slug: metabolon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-auth-api-openapi.yml
- filename: metabolon-decentralization-api-openapi.yml
  format: yaml
  label: Metabolon Decentralization API
  slug: metabolon-decentralization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-decentralization-api-openapi.yml
- filename: metabolon-eula-api-openapi.yml
  format: yaml
  label: Metabolon Eula API
  slug: metabolon-eula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-eula-api-openapi.yml
- filename: metabolon-files-api-openapi.yml
  format: yaml
  label: Metabolon Files API
  slug: metabolon-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-files-api-openapi.yml
- filename: metabolon-health-api-openapi.yml
  format: yaml
  label: Metabolon Health API
  slug: metabolon-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-health-api-openapi.yml
- filename: metabolon-labvantagefiles-api-openapi.yml
  format: yaml
  label: Metabolon Lab Vantage Files API
  slug: metabolon-labvantagefiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-labvantagefiles-api-openapi.yml
- filename: metabolon-pipelinestatus-api-openapi.yml
  format: yaml
  label: Metabolon Pipeline Status API
  slug: metabolon-pipelinestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-pipelinestatus-api-openapi.yml
- filename: metabolon-projects-api-openapi.yml
  format: yaml
  label: Metabolon Projects API
  slug: metabolon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-projects-api-openapi.yml
- filename: metabolon-reports-api-openapi.yml
  format: yaml
  label: Metabolon Reports API
  slug: metabolon-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-reports-api-openapi.yml
- filename: metabolon-samplesets-api-openapi.yml
  format: yaml
  label: Metabolon Sample Sets API
  slug: metabolon-samplesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-samplesets-api-openapi.yml
- filename: metabolon-samplesetsinfo-api-openapi.yml
  format: yaml
  label: Metabolon Sample Sets Info API
  slug: metabolon-samplesetsinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-samplesetsinfo-api-openapi.yml
- filename: metabolon-search-api-openapi.yml
  format: yaml
  label: Metabolon Search API
  slug: metabolon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-search-api-openapi.yml
- filename: metabolon-sharedfile-api-openapi.yml
  format: yaml
  label: Metabolon Shared File API
  slug: metabolon-sharedfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-sharedfile-api-openapi.yml
- filename: metabolon-spectraldata-api-openapi.yml
  format: yaml
  label: Metabolon Spectral Data API
  slug: metabolon-spectraldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-spectraldata-api-openapi.yml
- filename: metabolon-status-api-openapi.yml
  format: yaml
  label: Metabolon Status API
  slug: metabolon-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-status-api-openapi.yml
- filename: metabolon-studybuilder-api-openapi.yml
  format: yaml
  label: Metabolon Study Builder API
  slug: metabolon-studybuilder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-studybuilder-api-openapi.yml
- filename: metabolon-users-api-openapi.yml
  format: yaml
  label: Metabolon Users API
  slug: metabolon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Metabolon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metabolon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Metabolon
provider_slug: metabolon
scheme_count: 1
schemes:
- backchannel_logout_supported: true
  discovery_file: well-known/metabolon-openid-configuration.json
  endpoints:
    authorization: https://auth0.metabolon.com/authorize
    device_authorization: https://auth0.metabolon.com/oauth/device/code
    jwks: https://auth0.metabolon.com/.well-known/jwks.json
    mfa_challenge: https://auth0.metabolon.com/mfa/challenge
    registration: https://auth0.metabolon.com/oidc/register
    revocation: https://auth0.metabolon.com/oauth/revoke
    token: https://auth0.metabolon.com/oauth/token
    userinfo: https://auth0.metabolon.com/userinfo
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_algs:
  - RS256
  - HS256
  - PS256
  mfa:
    evidence: mfa_challenge_endpoint present plus mfa-oob / mfa-otp / mfa-recovery-code grant types
    supported: true
  name: Auth0 OIDC
  openIdConnectUrl: https://auth0.metabolon.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  request_uri_parameter_supported: false
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  scopes: scopes/metabolon-scopes.yml
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: metabolon-authentication
source_filename: metabolon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://auth0.metabolon.com/.well-known/openid-configuration\ndocs: https://www.metabolon.com/support/portal/data/\nnote: >-\n  The publicly served PortalApi OpenAPI declares NO components.securitySchemes and no top-level security\n  requirement, so nothing could be derived from the contract — derive-authentication.py returned zero\n  schemes. The auth model below is read from the live OIDC discovery document on Metabolon's own Auth0\n  custom domain (auth0.metabolon.com) plus the Auth0 SPA client wired into the portal.metabolon.com React\n  bundle. Metabolon publishes no developer authentication documentation; there is no API key programme, no\n  self-service credential issuance, and no machine/service-account path documented anywhere public.\nsummary:\n  model: oauth2-oidc\n  provider: Auth0 (Metabolon-branded custom domain)\n  issuer: https://auth0.metabolon.com/\n  legacy_issuer: https://metabolon.auth0.com/\n  runtime_credential:\
  \ Bearer JWT (RS256) presented to the *.prod.metabolon.com services\n  self_service: false\n  api_keys: false\n  mtls: false\n  declared_in_spec: false\nschemes:\n- name: Auth0 OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth0.metabolon.com/.well-known/openid-configuration\n  discovery_file: well-known/metabolon-openid-configuration.json\n  endpoints:\n    authorization: https://auth0.metabolon.com/authorize\n    token: https://auth0.metabolon.com/oauth/token\n    userinfo: https://auth0.metabolon.com/userinfo\n    jwks: https://auth0.metabolon.com/.well-known/jwks.json\n    revocation: https://auth0.metabolon.com/oauth/revoke\n    registration: https://auth0.metabolon.com/oidc/register\n    device_authorization: https://auth0.metabolon.com/oauth/device/code\n    mfa_challenge: https://auth0.metabolon.com/mfa/challenge\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs:\n  - RS256\n  - HS256\n  - PS256\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  mfa:\n    supported: true\n    evidence: mfa_challenge_endpoint present plus mfa-oob / mfa-otp / mfa-recovery-code grant types\n  backchannel_logout_supported: true\n  request_uri_parameter_supported: false\n  scopes: scopes/metabolon-scopes.yml\n\
  identity_flows:\n- name: Portal sign-in\n  description: Auth0 SPA authorization-code + PKCE flow initiated from https://portal.metabolon.com/login; the resulting access token is sent as a bearer credential to portal-api.prod.metabolon.com.\n  evidence: auth0-spa-js bundled in portal.metabolon.com/static/js/main.63f8c925.js\n- name: Pre-user-registration hook\n  description: Auth0 Action calls POST /api/v1/auth0/pre-user-registration on the Portal API to gate who may create an account.\n  operation: openapi/metabolon-portal-api-openapi.yml#Auth_OnPreUserRegistration\n- name: Post-login hook\n  description: Auth0 Action calls POST /api/v1/auth0/post-login on the Portal API after successful authentication.\n  operation: openapi/metabolon-portal-api-openapi.yml#Auth_OnPostLogin\n- name: Salesforce connection verification\n  description: GET /api/v1/auth0/verify-salesforce confirms the authenticating user maps to a Salesforce record; unapproved users go through an admin approval queue.\n  operation:\
  \ openapi/metabolon-portal-api-openapi.yml#Auth_VerifySalesforceConnection\n- name: Authorized context\n  description: GET /api/v1/auth/context returns the caller's resolved roles, permissions and project entitlements (IAuthorizedContext).\n  operation: openapi/metabolon-portal-api-openapi.yml#Auth_GetAuthorizedContext\n- name: Learning centre authorization\n  description: POST /api/v1/auth0/learning-center/authorize brokers access to the TalentLMS learning centre.\n  operation: openapi/metabolon-portal-api-openapi.yml#Auth_AuthorizeLearningCenterAccess\n- name: Assistant token exchange\n  description: POST /api/v1/assistant/token/{tenant} mints a scoped token for the in-portal assistant per tenant.\n  operation: openapi/metabolon-portal-api-openapi.yml#Assistant_GetToken\nauthorization:\n  model: role-and-project entitlement\n  note: >-\n    Authorization is enforced per project, not per scope. A user is granted membership of specific projects\n    (UserProject) and named roles carrying\
  \ permissions from a server-side catalog\n    (GET /api/v1/admin/users/roles/permissions/catalog). OAuth scopes on the token are the stock Auth0 OIDC\n    profile scopes and carry no API authorization meaning.\n  permission_catalog_operation: openapi/metabolon-portal-api-openapi.yml#Users_GetPermissionsCatalog\n  role_operations:\n  - openapi/metabolon-portal-api-openapi.yml#Users_GetRoles\n  - openapi/metabolon-portal-api-openapi.yml#Users_GetRolePermissions\n  - openapi/metabolon-portal-api-openapi.yml#Users_AddRolePermission\n  - openapi/metabolon-portal-api-openapi.yml#Users_RemoveRolePermission\ntransport_security:\n  tls: TLSv1.3 on every probed host\n  hsts: enabled on www.metabolon.com (max-age 31536000); absent on the *.prod.metabolon.com API hosts\n  encryption_at_rest: stated on https://www.metabolon.com/support/portal/data/\n  source: security/metabolon-domain-security.yml\ngaps:\n- No securitySchemes are declared in any of the four published OpenAPI documents.\n- No public\
  \ developer authentication documentation, no API key issuance, no documented service-account or client-credentials path for customers.\n- The published OpenAPI is served unauthenticated, but every non-health operation it describes requires a portal account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/authentication/metabolon-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Metabolomics
- Life Sciences
- Bioinformatics
- Multiomics
- Biotechnology
- Drug Discovery
- Precision Medicine
- Microbiome
- Biomarkers
- Contract Research
- Laboratory
---
