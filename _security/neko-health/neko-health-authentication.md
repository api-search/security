---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Neko Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
- ciba
overview: Neko Health secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, deviceCode, and ciba flow(s).
provider_name: Neko Health
provider_slug: neko-health
scheme_count: 1
schemes:
- authorization_endpoint: https://account.nekohealth.com/connect/authorize
  device_authorization_endpoint: https://account.nekohealth.com/connect/deviceauthorization
  end_session_endpoint: https://account.nekohealth.com/connect/endsession
  id_token_signing_alg: RS256
  introspection_endpoint: https://account.nekohealth.com/connect/introspect
  issuer: https://account.nekohealth.com
  name: NekoOIDC
  openIdConnectUrl: https://account.nekohealth.com/.well-known/openid-configuration
  pushed_authorization_request_endpoint: https://account.nekohealth.com/connect/par
  revocation_endpoint: https://account.nekohealth.com/connect/revocation
  scopes:
  - openid
  - profile
  - api.backend
  - offline_access
  token_endpoint: https://account.nekohealth.com/connect/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://account.nekohealth.com/connect/userinfo
slug: neko-health-authentication
source_filename: neko-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://account.nekohealth.com/.well-known/openid-configuration\ndocs: https://account.nekohealth.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the live Duende IdentityServer OIDC discovery document at\n  account.nekohealth.com. This is the identity provider for the Neko patient\n  application (client_id patientui); Neko publishes no third-party developer API.\n  No OpenAPI is available in the repo, so this profile is captured from the\n  discovery metadata rather than from securitySchemes.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - deviceCode\n  - ciba\n  pkce: true\n  login_methods:\n  - phone\n  - bankid\nschemes:\n- name: NekoOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://account.nekohealth.com/.well-known/openid-configuration\n  issuer: https://account.nekohealth.com\n  authorization_endpoint: https://account.nekohealth.com/connect/authorize\n\
  \  token_endpoint: https://account.nekohealth.com/connect/token\n  userinfo_endpoint: https://account.nekohealth.com/connect/userinfo\n  end_session_endpoint: https://account.nekohealth.com/connect/endsession\n  revocation_endpoint: https://account.nekohealth.com/connect/revocation\n  introspection_endpoint: https://account.nekohealth.com/connect/introspect\n  device_authorization_endpoint: https://account.nekohealth.com/connect/deviceauthorization\n  pushed_authorization_request_endpoint: https://account.nekohealth.com/connect/par\n  id_token_signing_alg: RS256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  scopes:\n  - openid\n  - profile\n  - api.backend\n  - offline_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neko-health/refs/heads/main/authentication/neko-health-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Health
- Healthcare
- Preventive Health
- Medical
- Body Scan
- Diagnostics
- Consumer Health
- OpenID Connect
---
