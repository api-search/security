---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Strata Identity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Strata Identity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Strata Identity
provider_slug: strata-identity
scheme_count: 1
schemes:
- assertion:
    claims:
      aud: the region token endpoint URL
      exp: future expiry timestamp
      iss: client ID
      sub: must equal iss (the client ID)
    header:
      alg: ES256
      typ: JWT
    signing_alg: ES256
    spec: RFC 7523 (JWT client assertion)
  client_authentication: private_key_jwt
  discovery:
    method: OpenID Connect discovery
    uk: https://auth.eu-west-2.strata.io/.well-known/openid-configuration
    us: https://auth.us-east-2.strata.io/.well-known/openid-configuration
  flow: clientCredentials
  grant: client_credentials
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:token-exchange
  name: MavericsConsoleOAuth2
  scopes_supported:
  - openid
  - profile
  - email
  - phone
  - offline_access
  token_endpoint_us: https://auth.us-east-2.strata.io/oauth2/token
  type: oauth2
slug: strata-identity-authentication
source_filename: strata-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.strata.io/reference/console/api-clients\ndocs: https://docs.strata.io/reference/console/api-clients\nnotes: >-\n  Auth profile for the Maverics Console public management API. Strata publishes no\n  machine-readable OpenAPI for this API, so this profile is captured from the docs\n  and the live regional OpenID Connect discovery documents rather than derived from\n  a spec. API clients are confidential OAuth 2.0 clients using the client-credentials\n  grant with private_key_jwt (JWT client assertion) authentication.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  client_auth_methods:\n  - private_key_jwt\n  assertion_alg: ES256\nschemes:\n- name: MavericsConsoleOAuth2\n  type: oauth2\n  flow: clientCredentials\n  grant: client_credentials\n  client_authentication: private_key_jwt\n  assertion:\n    spec: RFC 7523 (JWT client assertion)\n    signing_alg: ES256\n    header: {alg: ES256, typ:\
  \ JWT}\n    claims:\n      iss: client ID\n      sub: must equal iss (the client ID)\n      aud: the region token endpoint URL\n      exp: future expiry timestamp\n  discovery:\n    method: OpenID Connect discovery\n    us: https://auth.us-east-2.strata.io/.well-known/openid-configuration\n    uk: https://auth.eu-west-2.strata.io/.well-known/openid-configuration\n  token_endpoint_us: https://auth.us-east-2.strata.io/oauth2/token\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - phone\n  - offline_access\nidentity_orchestration:\n  note: >-\n    Separately, the Maverics Orchestrator federates end-user auth to any upstream\n    identity provider via its Identity Fabric connectors (SAML, OIDC, LDAP, Active\n    Directory, OAuth). These are the auth protocols the product brokers for\n    protected applications,\
  \ distinct from the Console API's own client auth above.\n  protocols:\n  - SAML 2.0\n  - OpenID Connect\n  - OAuth 2.0\n  - LDAP\n  - Active Directory\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strata-identity/refs/heads/main/authentication/strata-identity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Identity
- Identity Orchestration
- Authentication
- Authorization
- Single Sign-On
- IAM
- OAuth
- SAML
- OpenID Connect
- AI Identity
- Security
---
