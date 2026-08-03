---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Bostongene Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: BostonGene secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: BostonGene
provider_slug: bostongene
scheme_count: 1
schemes:
- dynamic_client_registration: true
  endpoints:
    authorization: https://bostongene.my.site.com/services/oauth2/authorize
    end_session: https://bostongene.my.site.com/services/auth/idp/oidc/logout
    introspection: https://bostongene.my.site.com/services/oauth2/introspect
    jwks: https://bostongene.my.site.com/id/keys
    registration: https://bostongene.my.site.com/services/oauth2/register
    revocation: https://bostongene.my.site.com/services/oauth2/revoke
    token: https://bostongene.my.site.com/services/oauth2/token
    userinfo: https://bostongene.my.site.com/services/oauth2/userinfo
  frontchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://bostongene.my.site.com
  name: BostonGene Customer Portal (OIDC)
  openIdConnectUrl: https://bostongene.my.site.com/.well-known/openid-configuration
  platform: Salesforce Experience Cloud
  response_types_supported:
  - code
  - token
  - token id_token
  scopes: scopes/bostongene-scopes.yml
  sources:
  - well-known/bostongene-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: bostongene-authentication
source_filename: bostongene-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://bostongene.my.site.com/.well-known/openid-configuration\ndocs: https://bostongene.com/new-account-request\nnote: >-\n  BostonGene publishes no developer API and therefore no API authentication\n  documentation. The only machine-readable authentication contract observable on\n  a BostonGene-controlled host is the OpenID Connect discovery document served by\n  the BostonGene Customer Portal, a Salesforce Experience Cloud site. The\n  endpoints below are BostonGene-branded (issuer = https://bostongene.my.site.com)\n  but the flows, scopes and claims are the Salesforce platform's, not a\n  BostonGene-designed API authorization model. Portal accounts are provisioned by\n  request for clinicians, PAs, nurse practitioners and pathologists — there is no\n  self-service developer key issuance.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  developer_api_auth:\
  \ none-published\nschemes:\n- name: BostonGene Customer Portal (OIDC)\n  type: openIdConnect\n  openIdConnectUrl: https://bostongene.my.site.com/.well-known/openid-configuration\n  issuer: https://bostongene.my.site.com\n  platform: Salesforce Experience Cloud\n  sources:\n  - well-known/bostongene-openid-configuration.json\n  endpoints:\n    authorization: https://bostongene.my.site.com/services/oauth2/authorize\n    token: https://bostongene.my.site.com/services/oauth2/token\n    userinfo: https://bostongene.my.site.com/services/oauth2/userinfo\n    revocation: https://bostongene.my.site.com/services/oauth2/revoke\n    introspection: https://bostongene.my.site.com/services/oauth2/introspect\n    registration: https://bostongene.my.site.com/services/oauth2/register\n    jwks: https://bostongene.my.site.com/id/keys\n    end_session: https://bostongene.my.site.com/services/auth/idp/oidc/logout\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  token_endpoint_auth_methods_supported:\n\
  \  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  frontchannel_logout_supported: true\n  dynamic_client_registration: true\n  scopes: scopes/bostongene-scopes.yml\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://bostongene.my.site.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bostongene/refs/heads/main/authentication/bostongene-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Health Care
- Oncology
- Precision Medicine
- Genomics
- Bioinformatics
- Artificial Intelligence
- Diagnostics
- Life Sciences
- Clinical Laboratory
---
