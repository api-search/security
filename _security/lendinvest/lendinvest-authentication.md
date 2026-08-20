---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Lendinvest Authentication
name_suffix: Authentication
oauth_flows: []
overview: LendInvest declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LendInvest
provider_slug: lendinvest
scheme_count: 1
schemes:
- claims_supported:
  - sub
  - user_id
  - organization_id
  - user_type
  - name
  - given_name
  - family_name
  - preferred_username
  - nickname
  - email
  - email_verified
  - phone_number
  - phone_number_verified
  - address
  - profile
  - picture
  - photos
  - urls
  - locale
  - language
  - zoneinfo
  - updated_at
  - is_app_installed
  - active
  discovery_url: https://customerportal.lendinvest.com/.well-known/openid-configuration
  dynamic_client_registration: true
  endpoints:
    authorization: https://customerportal.lendinvest.com/services/oauth2/authorize
    end_session: https://customerportal.lendinvest.com/services/auth/idp/oidc/logout
    introspection: https://customerportal.lendinvest.com/services/oauth2/introspect
    jwks: https://customerportal.lendinvest.com/id/keys
    registration: https://customerportal.lendinvest.com/services/oauth2/register
    revocation: https://customerportal.lendinvest.com/services/oauth2/revoke
    token: https://customerportal.lendinvest.com/services/oauth2/token
    userinfo: https://customerportal.lendinvest.com/services/oauth2/userinfo
  frontchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://customerportal.lendinvest.com
  name: openid_connect
  platform: Salesforce Experience Cloud
  refresh_tokens: true
  response_types_supported:
  - code
  - token
  - token id_token
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: lendinvest-authentication
source_filename: lendinvest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://customerportal.lendinvest.com/.well-known/openid-configuration\ndocs: https://customerportal.lendinvest.com/s/\nsummary: >-\n  LendInvest exposes no public developer API and therefore no public API authentication\n  surface. The only machine-readable authentication contract on the estate is the OpenID\n  Connect discovery document published by customerportal.lendinvest.com, the Salesforce\n  Experience Cloud community that fronts the LendInvest broker and borrower Mortgages\n  Portal. It advertises a standard Salesforce OAuth 2.0 / OIDC authorization server. The\n  endpoints and capabilities below are captured verbatim from that document; they govern\n  portal sign-in and any Salesforce-connected-app integration a partner is granted, not a\n  public LendInvest product API.\npublic_api: false\nschemes:\n- name: openid_connect\n  type: openIdConnect\n  issuer: https://customerportal.lendinvest.com\n  discovery_url: https://customerportal.lendinvest.com/.well-known/openid-configuration\n\
  \  platform: Salesforce Experience Cloud\n  endpoints:\n    authorization: https://customerportal.lendinvest.com/services/oauth2/authorize\n    token: https://customerportal.lendinvest.com/services/oauth2/token\n    userinfo: https://customerportal.lendinvest.com/services/oauth2/userinfo\n    revocation: https://customerportal.lendinvest.com/services/oauth2/revoke\n    introspection: https://customerportal.lendinvest.com/services/oauth2/introspect\n    registration: https://customerportal.lendinvest.com/services/oauth2/register\n    end_session: https://customerportal.lendinvest.com/services/auth/idp/oidc/logout\n    jwks: https://customerportal.lendinvest.com/id/keys\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  dynamic_client_registration: true\n  frontchannel_logout_supported:\
  \ true\n  refresh_tokens: true\n  claims_supported:\n  - sub\n  - user_id\n  - organization_id\n  - user_type\n  - name\n  - given_name\n  - family_name\n  - preferred_username\n  - nickname\n  - email\n  - email_verified\n  - phone_number\n  - phone_number_verified\n  - address\n  - profile\n  - picture\n  - photos\n  - urls\n  - locale\n  - language\n  - zoneinfo\n  - updated_at\n  - is_app_installed\n  - active\nscopes_artifact: scopes/lendinvest-scopes.yml\nrelated:\n  well_known: well-known/lendinvest-well-known.yml\n  conformance: conformance/lendinvest-conformance.yml\n  domain_security: security/lendinvest-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendinvest/refs/heads/main/authentication/lendinvest-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Lending
- Mortgages
- Property Finance
- Real-Estate
- Financial-Services
- United Kingdom
---
