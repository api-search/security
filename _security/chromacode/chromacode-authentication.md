---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Chromacode Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- deviceCode
- ciba
overview: ChromaCode secures its APIs with openIdConnect, oauth2, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, deviceCode, and ciba flow(s).
provider_name: ChromaCode
provider_slug: chromacode
scheme_count: 2
schemes:
- backchannel_logout_supported: true
  description: Primary realm used by the ChromaCode Cloud browser application. The public client "production-frontend" performs authorization_code with PKCE (check-sso on load) against this realm, brokered to the "production-idp" identity provider.
  endpoints:
    authorization: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth
    backchannel_authentication: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/ext/ciba/auth
    device_authorization: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth/device
    end_session: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/logout
    introspection: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token/introspect
    jwks: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/certs
    pushed_authorization_request: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/ext/par/request
    registration: https://openid.chromacodecloud.com/auth/realms/apps/clients-registrations/openid-connect
    revocation: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/revoke
    token: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token
    userinfo: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/userinfo
  frontchannel_logout_supported: true
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_signing_algs:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  issuer: https://openid.chromacodecloud.com/auth/realms/apps
  mtls_bound_access_tokens: true
  name: ChromaCodeCloudOIDC
  openIdConnectUrl: https://openid.chromacodecloud.com/auth/realms/apps/.well-known/openid-configuration
  pkce_methods:
  - plain
  - S256
  realm: apps
  require_pushed_authorization_requests: false
  sources:
  - well-known/chromacode-openid-configuration-apps.json
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
- description: Secondary "cloud" user realm referenced as userRealm by the ChromaCode Cloud runtime config. Same Keycloak capability set as the apps realm but without the chromacloud application scopes.
  endpoints:
    authorization: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/auth
    jwks: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/certs
    token: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/token
    userinfo: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/userinfo
  issuer: https://openid.chromacodecloud.com/auth/realms/cloud
  name: ChromaCodeCloudUserRealmOIDC
  openIdConnectUrl: https://openid.chromacodecloud.com/auth/realms/cloud/.well-known/openid-configuration
  realm: cloud
  sources:
  - well-known/chromacode-openid-configuration-cloud.json
  type: openIdConnect
slug: chromacode-authentication
source_filename: chromacode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://openid.chromacodecloud.com/auth/realms/apps/.well-known/openid-configuration\ndocs: https://www.chromacode.com/chromacode-cloud/\nnote: >-\n  ChromaCode publishes no OpenAPI definition and no developer authentication guide,\n  so this profile is built from the provider's own publicly readable OpenID Connect\n  discovery documents plus the unauthenticated ChromaCode Cloud runtime config at\n  https://chromacodecloud.com/config, and confirmed against the observed HTTP 401\n  responses on every https://chromacodecloud.com/api/* path.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - password\n  - deviceCode\n  - ciba\n  identity_provider: Keycloak\n  public_api_key_program: false\nschemes:\n- name: ChromaCodeCloudOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://openid.chromacodecloud.com/auth/realms/apps/.well-known/openid-configuration\n\
  \  issuer: https://openid.chromacodecloud.com/auth/realms/apps\n  realm: apps\n  description: >-\n    Primary realm used by the ChromaCode Cloud browser application. The public\n    client \"production-frontend\" performs authorization_code with PKCE (check-sso\n    on load) against this realm, brokered to the \"production-idp\" identity provider.\n  sources:\n  - well-known/chromacode-openid-configuration-apps.json\n  endpoints:\n    authorization: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth\n    token: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token\n    userinfo: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/userinfo\n    jwks: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/certs\n    introspection: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token/introspect\n    revocation: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/revoke\n\
  \    end_session: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/logout\n    registration: https://openid.chromacodecloud.com/auth/realms/apps/clients-registrations/openid-connect\n    device_authorization: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth/device\n    pushed_authorization_request: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/ext/par/request\n    backchannel_authentication: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/ext/ciba/auth\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  pkce_methods:\n  - plain\n  - S256\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  id_token_signing_algs:\n  - RS256\n  -\
  \ RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\n  - HS256\n  - HS384\n  - HS512\n  mtls_bound_access_tokens: true\n  require_pushed_authorization_requests: false\n  backchannel_logout_supported: true\n  frontchannel_logout_supported: true\n- name: ChromaCodeCloudUserRealmOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://openid.chromacodecloud.com/auth/realms/cloud/.well-known/openid-configuration\n  issuer: https://openid.chromacodecloud.com/auth/realms/cloud\n  realm: cloud\n  description: >-\n    Secondary \"cloud\" user realm referenced as userRealm by the ChromaCode Cloud\n    runtime config. Same Keycloak capability set as the apps realm but without the\n    chromacloud application scopes.\n  sources:\n  - well-known/chromacode-openid-configuration-cloud.json\n  endpoints:\n    authorization: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/auth\n    token: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/token\n\
  \    userinfo: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/userinfo\n    jwks: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/certs\nclient:\n  id: production-frontend\n  public_client: true\n  on_load: check-sso\n  idp_hint: production-idp\n  redirect_uri: https://production.chromacodecloud.com\n  ssl_required: external\n  verify_token_audience: true\n  source: https://chromacodecloud.com/config\nobserved:\n- url: https://chromacodecloud.com/api/instrument\n  status: 401\n  body: '{\"message\":\"Authorization not present on request.\",\"error\":{\"name\":\"UnauthorizedError\"}}'\n- url: https://chromacodecloud.com/api/configuration/siteBanners\n  status: 401\n  body: '{\"message\":\"Authorization not present on request.\",\"error\":{\"name\":\"UnauthorizedError\"}}'\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - https://openid.chromacodecloud.com/auth/realms/apps/.well-known/openid-configuration\n  - https://openid.chromacodecloud.com/auth/realms/cloud/.well-known/openid-configuration\n\
  \  - https://chromacodecloud.com/config\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chromacode/refs/heads/main/authentication/chromacode-authentication.yml
summary_line: openIdConnect/oauth2/mutualTLS · 2 schemes
tags:
- Company
- Molecular Diagnostics
- Genomics
- Oncology
- PCR
- Life Sciences
- Healthcare
- Bioinformatics
- Clinical Diagnostics
- Cloud Software
---
