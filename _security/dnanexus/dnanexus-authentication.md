---
api_key_in: []
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Dnanexus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DNAnexus secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DNAnexus
provider_slug: dnanexus
scheme_count: 3
schemes:
- applies_to: https://api.dnanexus.com (all ~206 Platform API methods)
  errors:
  - http_status: 401
    message: You need to be logged in to use this method
    observed: 2026-08-04 POST https://api.dnanexus.com/system/whoami with empty body
    type: InvalidAuthentication
  - http_status: 401
    type: PermissionDenied
  format: 'Authorization: Bearer <token>'
  header: Authorization
  in: header
  name: PlatformBearerToken
  scheme: bearer
  source: https://documentation.dnanexus.com/developer/api/authentication
  token_kinds:
  - description: Issued when a user logs in through the UI or `dx login`.
    kind: interactive-login token
  - description: Created and revoked by the user in the platform web interface under username dropdown > Profile > API Tokens. This is the token developers use for scripted/programmatic access.
    kind: API token
    management_url: https://platform.dnanexus.com/
  - description: Automatically supplied to jobs in the Execution Environment; derived from the launching user's login or API token. Job authentication tokens are valid for at most 30 days, and a job in a job tree inherits the root execution's token expiration.
    kind: job token
    source: https://documentation.dnanexus.com/developer/apps/error-information
  type: http
- authorization_endpoint: https://oidc.dnanexus.com/authorize
  claims_supported:
  - sub
  - name
  - email
  - user_id
  - sid
  - auth_time
  - iss
  code_challenge_methods_supported:
  - S256
  docs: https://documentation.dnanexus.com/developer/api/oidc-clients
  example_app: https://github.com/dnanexus/oidc-example-app
  file: well-known/dnanexus-oidc-openid-configuration.json
  grant_types_supported:
  - authorization_code
  issuer: https://oidc.dnanexus.com
  jwks_uri: https://oidc.dnanexus.com/jwks
  name: DNAnexusOIDC
  openIdConnectUrl: https://oidc.dnanexus.com/.well-known/openid-configuration
  purpose: Lets a third-party web application sign users in with their DNAnexus Platform credentials. OIDC clients are registered through the Platform API oidcClient methods (/oidcClient-xxxx/*).
  response_modes_supported:
  - form_post
  - fragment
  - query
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - name
  - email
  - user_id
  subject_types_supported:
  - pairwise
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- claims_supported:
  - sub
  - aud
  - exp
  - iat
  - iss
  - jti
  - nbf
  - job_id
  - root_execution_id
  - root_executable_id
  - root_executable_name
  - root_executable_version
  - executable_id
  - app_name
  - app_version
  - project_id
  - bill_to
  - launched_by
  - region
  - job_worker_ipv4
  - job_worker_ipv6
  - job_try
  docs: https://documentation.dnanexus.com/developer/apps/job-identity-tokens-for-access-to-clouds-and-third-party-services
  file: well-known/dnanexus-job-oidc-openid-configuration.json
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://job-oidc.dnanexus.com
  jwks_uri: https://job-oidc.dnanexus.com/.well-known/jwks
  name: DNAnexusJobIdentityToken
  openIdConnectUrl: https://job-oidc.dnanexus.com/.well-known/openid-configuration
  purpose: 'Workload identity federation: a running DNAnexus job requests an OIDC ID token (via /job-xxxx/getIdentityToken or dx-jobutil-get-identity-token) and exchanges it with AWS/Azure/GCP or another third-party service, so apps do not carry long lived cloud credentials.'
  response_types_supported:
  - id_token
  scopes_supported:
  - openid
  subject_types_supported:
  - public
  - pairwise
  type: openIdConnect
slug: dnanexus-authentication
source_filename: dnanexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://documentation.dnanexus.com/developer/api/authentication\ndocs: https://documentation.dnanexus.com/developer/api/authentication\nnote: >-\n  DNAnexus publishes no OpenAPI/Swagger definition, so this profile was read from\n  the provider's own API documentation and from the live OIDC discovery documents\n  rather than derived from securitySchemes.\nsummary:\n  types: [http, openIdConnect]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\nschemes:\n- name: PlatformBearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  applies_to: https://api.dnanexus.com (all ~206 Platform API methods)\n  source: https://documentation.dnanexus.com/developer/api/authentication\n  token_kinds:\n  - kind: interactive-login token\n    description: Issued when a user logs in through the UI or `dx login`.\n  - kind: API token\n    description:\
  \ >-\n      Created and revoked by the user in the platform web interface under\n      username dropdown > Profile > API Tokens. This is the token developers use\n      for scripted/programmatic access.\n    management_url: https://platform.dnanexus.com/\n  - kind: job token\n    description: >-\n      Automatically supplied to jobs in the Execution Environment; derived from\n      the launching user's login or API token. Job authentication tokens are valid\n      for at most 30 days, and a job in a job tree inherits the root execution's\n      token expiration.\n    source: https://documentation.dnanexus.com/developer/apps/error-information\n  errors:\n  - type: InvalidAuthentication\n    http_status: 401\n    message: You need to be logged in to use this method\n    observed: '2026-08-04 POST https://api.dnanexus.com/system/whoami with empty body'\n  - type: PermissionDenied\n    http_status: 401\n- name: DNAnexusOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://oidc.dnanexus.com/.well-known/openid-configuration\n\
  \  issuer: https://oidc.dnanexus.com\n  purpose: >-\n    Lets a third-party web application sign users in with their DNAnexus Platform\n    credentials. OIDC clients are registered through the Platform API oidcClient\n    methods (/oidcClient-xxxx/*).\n  docs: https://documentation.dnanexus.com/developer/api/oidc-clients\n  example_app: https://github.com/dnanexus/oidc-example-app\n  authorization_endpoint: https://oidc.dnanexus.com/authorize\n  jwks_uri: https://oidc.dnanexus.com/jwks\n  grant_types_supported: [authorization_code]\n  response_types_supported: [code]\n  response_modes_supported: [form_post, fragment, query]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  subject_types_supported: [pairwise]\n  scopes_supported: [openid, name, email, user_id]\n  claims_supported: [sub, name, email, user_id, sid, auth_time, iss]\n  file: well-known/dnanexus-oidc-openid-configuration.json\n- name: DNAnexusJobIdentityToken\n  type:\
  \ openIdConnect\n  openIdConnectUrl: https://job-oidc.dnanexus.com/.well-known/openid-configuration\n  issuer: https://job-oidc.dnanexus.com\n  purpose: >-\n    Workload identity federation: a running DNAnexus job requests an OIDC ID token\n    (via /job-xxxx/getIdentityToken or dx-jobutil-get-identity-token) and exchanges\n    it with AWS/Azure/GCP or another third-party service, so apps do not carry long\n    lived cloud credentials.\n  docs: https://documentation.dnanexus.com/developer/apps/job-identity-tokens-for-access-to-clouds-and-third-party-services\n  jwks_uri: https://job-oidc.dnanexus.com/.well-known/jwks\n  response_types_supported: [id_token]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public, pairwise]\n  scopes_supported: [openid]\n  claims_supported: [sub, aud, exp, iat, iss, jti, nbf, job_id, root_execution_id,\n    root_executable_id, root_executable_name, root_executable_version, executable_id,\n    app_name, app_version, project_id,\
  \ bill_to, launched_by, region, job_worker_ipv4,\n    job_worker_ipv6, job_try]\n  file: well-known/dnanexus-job-oidc-openid-configuration.json\nmfa:\n  supported: true\n  docs: https://documentation.dnanexus.com/user/login-and-logout\n  note: Two-factor authentication is documented on the login/logout page.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url: https://oidc.dnanexus.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://job-oidc.dnanexus.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://auth.dnanexus.com/.well-known/openid-configuration\n    http_status: 404\n  - url: https://api.dnanexus.com/system/whoami\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnanexus/refs/heads/main/authentication/dnanexus-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Company
- Genomics
- Bioinformatics
- Life Sciences
- Healthcare
- Cloud Computing
- Data Platform
- Scientific Computing
- Precision Medicine
- Clinical Research
---
