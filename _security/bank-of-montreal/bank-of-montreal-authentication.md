---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bank Of Montreal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- jwt-bearer
overview: BMO Financial Group secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and jwt-bearer flow(s).
provider_name: BMO Financial Group
provider_slug: bank-of-montreal
scheme_count: 3
schemes:
- description: OAuth 2.0 access tokens issued by the BMO Authorize API grant applications access to the Account Information, Account Validation, Image Retrieval, and Payment APIs across sandbox, pre-production, and production environments.
  flows:
  - authorizationUrl: https://api.bmo.com/aac/sps/oauth/oauth20/authorize
    flow: authorizationCode
    tokenUrl: https://api.bmo.com/aac/sps/oauth/oauth20/token
  - flow: jwt-bearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://api.bmo.com/aac/sps/oauth/oauth20/token
  name: OAuth2
  sources:
  - well-known/bank-of-montreal-openid-configuration.json
  type: oauth2
- grant_types_supported:
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://api.bmo.com/aac/sps/oauth/oauth20/introspect
  issuer: https://api.bmo.com
  jwks_uri: https://api.bmo.com/aac/sps/oauth/oauth20/jwks/VerifymeOIDC
  name: OpenIDConnect
  openIdConnectUrl: https://api.bmo.com/.well-known/openid-configuration
  provider: IBM Security Verify (VerifymeOIDC)
  response_types_supported:
  - code
  - none
  revocation_endpoint: https://api.bmo.com/aac/sps/oauth/oauth20/revoke
  sources:
  - well-known/bank-of-montreal-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://api.bmo.com/aac/sps/oauth/oauth20/userinfo
- description: The BMO Encryption API encrypts all requests to and responses from BMO APIs; encryption is mandatory for the Payment APIs and for fields shared via the Account Validation API. This is an application-layer requirement on top of OAuth 2.0 transport auth.
  name: Encryption
  sources:
  - https://developer.bmo.com/api/commercial/product
  type: message-encryption
slug: bank-of-montreal-authentication
source_filename: bank-of-montreal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://api.bmo.com/.well-known/openid-configuration (live OIDC discovery) +\n  https://developer.bmo.com/api/commercial/ (BMO Authorize API, OAuth 2.0)\ndocs: https://developer.bmo.com/api/commercial/product\nnotes: >-\n  Derived from BMO's live OIDC discovery document and the documented Authorize\n  API. Full per-endpoint OpenAPI security is partner-gated (an approved BMO\n  Online Banking for Business organization account is required to view the API\n  Explorer specs), so scheme details below are grounded in the anonymous OIDC\n  discovery endpoint plus the portal's published auth description.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, jwt-bearer]\n  oidc_issuer: https://api.bmo.com\n  encryption_required: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 access tokens issued by the BMO Authorize API grant applications\n    access to the Account Information,\
  \ Account Validation, Image Retrieval, and\n    Payment APIs across sandbox, pre-production, and production environments.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bmo.com/aac/sps/oauth/oauth20/authorize\n    tokenUrl: https://api.bmo.com/aac/sps/oauth/oauth20/token\n  - flow: jwt-bearer\n    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenUrl: https://api.bmo.com/aac/sps/oauth/oauth20/token\n  sources: [well-known/bank-of-montreal-openid-configuration.json]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.bmo.com/.well-known/openid-configuration\n  issuer: https://api.bmo.com\n  provider: IBM Security Verify (VerifymeOIDC)\n  userinfo_endpoint: https://api.bmo.com/aac/sps/oauth/oauth20/userinfo\n  jwks_uri: https://api.bmo.com/aac/sps/oauth/oauth20/jwks/VerifymeOIDC\n  introspection_endpoint: https://api.bmo.com/aac/sps/oauth/oauth20/introspect\n  revocation_endpoint: https://api.bmo.com/aac/sps/oauth/oauth20/revoke\n\
  \  id_token_signing_alg_values_supported: [RS256]\n  response_types_supported: [code, none]\n  grant_types_supported: [urn:ietf:params:oauth:grant-type:jwt-bearer, authorization_code]\n  sources: [well-known/bank-of-montreal-openid-configuration.json]\n- name: Encryption\n  type: message-encryption\n  description: >-\n    The BMO Encryption API encrypts all requests to and responses from BMO APIs;\n    encryption is mandatory for the Payment APIs and for fields shared via the\n    Account Validation API. This is an application-layer requirement on top of\n    OAuth 2.0 transport auth.\n  sources: [https://developer.bmo.com/api/commercial/product]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-montreal/refs/heads/main/authentication/bank-of-montreal-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Financial-Services
- Banking
- Canada
- Big Six
- Commercial Banking
- Payments
- Treasury
- Open Banking
- Consumer-Driven Banking
---
