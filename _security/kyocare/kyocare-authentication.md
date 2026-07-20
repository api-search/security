---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kyocare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Kyo secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Kyo
provider_slug: kyocare
scheme_count: 2
schemes:
- end_session_endpoint: https://auth.kyocare.com/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.attain.kyocare.com
  name: openIdConnect
  openIdConnectUrl: https://api.attain.kyocare.com/.well-known/openid-configuration
  sources:
  - well-known/kyocare-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://auth.kyocare.com/oauth2/userInfo
- flows:
  - authorizationUrl: https://api.attain.kyocare.com/oauth/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    refreshUrl: null
    tokenUrl: https://api.attain.kyocare.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.attain.kyocare.com/oauth/token
  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_DEP9DvC1P/.well-known/jwks.json
  name: oauth2
  registration_endpoint: https://api.attain.kyocare.com/register
  response_types_supported:
  - code
  - token
  revocation_endpoint: https://auth.kyocare.com/oauth2/revoke
  sources:
  - well-known/kyocare-openid-configuration.json
  - well-known/kyocare-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: kyocare-authentication
source_filename: kyocare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.attain.kyocare.com/.well-known/openid-configuration\ndocs: https://api.attain.kyocare.com/.well-known/openid-configuration\nnote: Derived from the live OIDC discovery + RFC 8414 authorization-server metadata\n  published by the Attain platform API. Kyo publishes no developer documentation; this\n  profile is read entirely from the machine-readable discovery documents.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  pkce: S256\n  identity_provider: AWS Cognito (us-east-1_DEP9DvC1P)\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.attain.kyocare.com/.well-known/openid-configuration\n  issuer: https://api.attain.kyocare.com\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  userinfo_endpoint: https://auth.kyocare.com/oauth2/userInfo\n  end_session_endpoint: https://auth.kyocare.com/logout\n\
  \  sources:\n  - well-known/kyocare-openid-configuration.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.attain.kyocare.com/oauth/authorize\n    tokenUrl: https://api.attain.kyocare.com/oauth/token\n    refreshUrl: null\n    pkce_methods:\n    - S256\n  - flow: clientCredentials\n    tokenUrl: https://api.attain.kyocare.com/oauth/token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  response_types_supported:\n  - code\n  - token\n  revocation_endpoint: https://auth.kyocare.com/oauth2/revoke\n  registration_endpoint: https://api.attain.kyocare.com/register\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_DEP9DvC1P/.well-known/jwks.json\n  sources:\n  - well-known/kyocare-openid-configuration.json\n  - well-known/kyocare-oauth-authorization-server.json\ngateways:\n- host: api.kyocare.com\n  vendor: Workato API Platform\n  evidence: CNAME apim-custom.workato.com;\
  \ server:envoy; x-gateway-version:1.27.1\n  access: private\n  observed_response: '401 {\"error\":\"access to this API has been disallowed\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyocare/refs/heads/main/authentication/kyocare-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Healthcare
- Autism
- ABA Therapy
- Behavioral Health
- Patient Engagement
- Digital Health
- Scheduling
- Private API
---
