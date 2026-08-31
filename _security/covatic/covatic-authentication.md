---
api_key_in: []
api_specs:
- filename: covatic-audience-builder-agent-api-openapi.yml
  format: yaml
  label: Covatic Audience Builder Agent API
  slug: covatic-audience-builder-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-audience-builder-agent-api-openapi.yml
- filename: covatic-audience-builder-api-openapi.yml
  format: yaml
  label: Covatic Audience Builder API
  slug: covatic-audience-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-audience-builder-api-openapi.yml
- filename: covatic-auth-api-openapi.yml
  format: yaml
  label: Covatic Auth API
  slug: covatic-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-auth-api-openapi.yml
- filename: covatic-campaigns-api-openapi.yml
  format: yaml
  label: Covatic Campaigns API
  slug: covatic-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-campaigns-api-openapi.yml
- filename: covatic-chatgpt-api-openapi.yml
  format: yaml
  label: Covatic Chat GPT API
  slug: covatic-chatgpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-chatgpt-api-openapi.yml
- filename: covatic-commons-api-openapi.yml
  format: yaml
  label: Covatic Commons API
  slug: covatic-commons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-commons-api-openapi.yml
- filename: covatic-company-api-openapi.yml
  format: yaml
  label: Covatic Company API
  slug: covatic-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-company-api-openapi.yml
- filename: covatic-event-traits-api-openapi.yml
  format: yaml
  label: Covatic Event Traits API
  slug: covatic-event-traits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-event-traits-api-openapi.yml
- filename: covatic-insights-api-openapi.yml
  format: yaml
  label: Covatic Insights API
  slug: covatic-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-insights-api-openapi.yml
- filename: covatic-notes-api-openapi.yml
  format: yaml
  label: Covatic Notes API
  slug: covatic-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-notes-api-openapi.yml
- filename: covatic-profiles-api-openapi.yml
  format: yaml
  label: Covatic Profiles API
  slug: covatic-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-profiles-api-openapi.yml
- filename: covatic-qa-and-debug-api-openapi.yml
  format: yaml
  label: Covatic QA and Debug API
  slug: covatic-qa-and-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-qa-and-debug-api-openapi.yml
- filename: covatic-retargeting-traits-api-openapi.yml
  format: yaml
  label: Covatic Retargeting Traits API
  slug: covatic-retargeting-traits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-retargeting-traits-api-openapi.yml
- filename: covatic-root-api-openapi.yml
  format: yaml
  label: Covatic Root API
  slug: covatic-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-root-api-openapi.yml
- filename: covatic-seeders-api-openapi.yml
  format: yaml
  label: Covatic Seeders API
  slug: covatic-seeders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-seeders-api-openapi.yml
- filename: covatic-tags-api-openapi.yml
  format: yaml
  label: Covatic Tags API
  slug: covatic-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-tags-api-openapi.yml
- filename: covatic-traits-api-openapi.yml
  format: yaml
  label: Covatic Traits API
  slug: covatic-traits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-traits-api-openapi.yml
- filename: covatic-users-api-openapi.yml
  format: yaml
  label: Covatic Users API
  slug: covatic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-users-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Covatic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Covatic secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Covatic
provider_slug: covatic
scheme_count: 2
schemes:
- applied_to_operations: 88
  header: Authorization
  in: header
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/covatic-audience-builder-openapi.yml
  type: http
  unauthenticated_note: Only GET / (the service banner) is public.
  unauthenticated_operations: 1
- authorization_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/authorize
  end_session_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/logout
  hosted_ui_domain: clienttoolsapi.auth.eu-west-2.amazoncognito.com
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg
  jwks_uri: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg/.well-known/jwks.json
  method: probed
  name: CognitoOIDC
  note: Discovered from the public JavaScript bundle Covatic serves at platform.covatic.io/assets/App-DtRW1Itl.js, which constructs a CognitoUserPool with UserPoolId eu-west-2_mQWqhJueg. The Cognito hosted-UI domain is `clienttoolsapi`, which matches the API root banner "Welcome to Covatic client tools." The SPA client id is public browser configuration and is deliberately not recorded here.
  openid_configuration: well-known/covatic-openid-configuration.json
  region: eu-west-2
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/revoke
  scopes_supported:
  - openid
  - email
  - phone
  - profile
  sources:
  - https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg/.well-known/openid-configuration
  token_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  user_pool_id: eu-west-2_mQWqhJueg
  userinfo_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/userInfo
slug: covatic-authentication
source_filename: covatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  openapi/covatic-audience-builder-openapi.yml (securitySchemes) +\n  https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg/.well-known/openid-configuration (HTTP 200) +\n  live 401 challenge from https://prodaudiencebuilderapi.covatic.io/api/v1/campaigns/\nsummary:\n  types:\n  - http\n  - openIdConnect\n  primary: HTTP Bearer token — an AWS Cognito (OIDC) ID/access JWT.\n  public_signup: false\n  note: >-\n    The Covatic Audience Builder API declares exactly one security scheme, HTTP Bearer.\n    The spec does not say where the token comes from; the platform SPA does. Covatic's\n    client platform authenticates against an AWS Cognito user pool in eu-west-2\n    (London) using amazon-cognito-identity-js, and sends the resulting JWT as\n    `Authorization: Bearer <token>`. Accounts are provisioned by Covatic — there is no\n    public sign-up, and users are created through the API's own\n    /api/v1/user/create-users-with-roles\
  \ and /api/v1/user/resend-invite operations.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  applied_to_operations: 88\n  unauthenticated_operations: 1\n  unauthenticated_note: Only GET / (the service banner) is public.\n  sources:\n  - openapi/covatic-audience-builder-openapi.yml\n- name: CognitoOIDC\n  type: openIdConnect\n  method: probed\n  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg\n  openid_configuration: well-known/covatic-openid-configuration.json\n  region: eu-west-2\n  user_pool_id: eu-west-2_mQWqhJueg\n  hosted_ui_domain: clienttoolsapi.auth.eu-west-2.amazoncognito.com\n  authorization_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/authorize\n  token_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/token\n  userinfo_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/userInfo\n  revocation_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/revoke\n\
  \  end_session_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/logout\n  jwks_uri: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\n  - RS256\n  response_types_supported:\n  - code\n  - token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  scopes_supported:\n  - openid\n  - email\n  - phone\n  - profile\n  sources:\n  - https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg/.well-known/openid-configuration\n  note: >-\n    Discovered from the public JavaScript bundle Covatic serves at\n    platform.covatic.io/assets/App-DtRW1Itl.js, which constructs a CognitoUserPool with\n    UserPoolId eu-west-2_mQWqhJueg. The Cognito hosted-UI domain is `clienttoolsapi`,\n    which matches the API root banner \"Welcome to Covatic client tools.\" The SPA client\n    id is public browser configuration and is deliberately not recorded here.\nchallenge_observed:\n\
  \  url: https://prodaudiencebuilderapi.covatic.io/api/v1/campaigns/\n  http_status: 401\n  body: '{\"detail\":\"Not authenticated\"}'\n  www_authenticate: null\n  note: >-\n    FastAPI's HTTPBearer returns a bare 401 JSON body with NO WWW-Authenticate header,\n    so an agent gets no machine-readable pointer to the token endpoint from the 401\n    itself. Adding `WWW-Authenticate: Bearer` (RFC 6750) or an\n    /.well-known/oauth-protected-resource document (RFC 9728) would close that gap.\nauthorization_model:\n  multi_tenant: true\n  tenant_parameter: client_id\n  note: >-\n    Most operations accept a `client_id` query parameter (34 operations) and users are\n    associated with one or more companies/clients; /api/v1/user/clients lists them and\n    /api/v1/user/clients/default/{default_client_id} sets the active tenant. Roles are\n    assigned at user creation (/api/v1/user/create-users-with-roles). The role\n    vocabulary itself is not published in the spec.\ndocs:\n  public: false\n\
  \  note: >-\n    Covatic's SDK/API documentation at docs.covatic.io is Wiki.js behind a login (403\n    for every unauthenticated path); covatic.com/technical/ tells existing clients to\n    email support@covatic.com for credentials. No public authentication guide exists.\ncross_links:\n  scopes: scopes/covatic-scopes.yml\n  conventions: conventions/covatic-conventions.yml\n  well_known: well-known/covatic-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/authentication/covatic-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Company
- Advertising Technology
- AdTech
- Audience Intelligence
- Data Management Platform
- Connected TV
- Privacy
- On-Device Processing
- Attribution
- Audio
- Campaigns
- Retargeting
- Publishing
- Broadcasting
- Media
- B Corp
- United Kingdom
---
