---
api_key_in:
- header
- cookie
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Appnexus Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppNexus secures its APIs with token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppNexus
provider_slug: appnexus
scheme_count: 2
schemes:
- carry:
  - 'Authorization: <TOKEN> request header'
  - session cookie (curl -b cookies -c cookies)
  error_signal: error_id NOAUTH in the response envelope signals re-authentication needed
  mechanism: username-password-token-exchange
  name: token
  obtain: POST https://api.appnexus.com/auth with JSON body {auth:{username,password}}; returns response.token
  reauth_limit: 10 successful authentications per 5-minute period
  reauth_limit_source: https://learn.microsoft.com/en-us/xandr/digital-platform-api/api-usage-constraints
  token_lifetime: 2 hours idle; 24-hour hard expiry regardless of activity
  type: token
- detail: '"For the Digital Platform API, we''ve implemented a signed token-based authentication system. This system uses JSON Web Tokens (JWT) to help ensure your sessions are as secure as possible."'
  docs: https://learn.microsoft.com/en-us/xandr/digital-platform-api/token-based-api-authentication
  mechanism: signed-token
  name: jwt
  type: token
slug: appnexus-authentication
source_filename: appnexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/xandr/digital-platform-api/authentication-service\ndocs:\n  - https://learn.microsoft.com/en-us/xandr/digital-platform-api/authentication-service\n  - https://learn.microsoft.com/en-us/xandr/digital-platform-api/token-based-api-authentication\n  - https://learn.microsoft.com/en-us/xandr/digital-platform-api/api-usage-constraints\nsummary:\n  types: [token]\n  scheme: custom-token\n  oauth2: false\n  oidc: false\n  jwt: true\n  api_key_in: [header, cookie]\n  scopes: false\n  scopes_note: >-\n    There is no OAuth scope surface. Authorization is role-based inside the platform - see\n    the Working with Roles using the API guide - and is not expressed in the credential.\nschemes:\n  - name: token\n    type: token\n    mechanism: username-password-token-exchange\n    obtain: \"POST https://api.appnexus.com/auth with JSON body {auth:{username,password}}; returns response.token\"\n    carry:\n\
  \      - \"Authorization: <TOKEN> request header\"\n      - \"session cookie (curl -b cookies -c cookies)\"\n    token_lifetime: \"2 hours idle; 24-hour hard expiry regardless of activity\"\n    reauth_limit: \"10 successful authentications per 5-minute period\"\n    reauth_limit_source: https://learn.microsoft.com/en-us/xandr/digital-platform-api/api-usage-constraints\n    error_signal: \"error_id NOAUTH in the response envelope signals re-authentication needed\"\n  - name: jwt\n    type: token\n    mechanism: signed-token\n    detail: >-\n      \"For the Digital Platform API, we've implemented a signed token-based authentication\n      system. This system uses JSON Web Tokens (JWT) to help ensure your sessions are as\n      secure as possible.\"\n    docs: https://learn.microsoft.com/en-us/xandr/digital-platform-api/token-based-api-authentication\naccount_recovery:\n  service: Account Recovery Service\n  docs: https://learn.microsoft.com/en-us/xandr/digital-platform-api/account-recovery-service\n\
  auth_errors:\n  - id: NOAUTH\n    meaning: not logged in, or credentials invalid\n  - id: NOAUTH_DISABLED\n    meaning: account deactivated\n  - id: NOAUTH_EXPIRED\n    meaning: password expired and needs reset\n  - id: UNAUTH\n    meaning: authenticated but not authorized for the requested action\ndiscovery:\n  well_known_openid_configuration: 404\n  well_known_oauth_authorization_server: 404\n  note: >-\n    No discovery document is served on api.appnexus.com; a client must be told the /auth\n    endpoint out of band. See well-known/appnexus-well-known.yml.\naccess_gate:\n  self_serve: false\n  note: >-\n    Credentials are issued only to existing Xandr/Microsoft Monetize customers through the\n    API Onboarding Process. See sandbox/appnexus-sandbox.yml.\ncross_links:\n  conventions: conventions/appnexus-conventions.yml\n  errors: errors/appnexus-error-codes.yml\n  conformance: conformance/appnexus-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appnexus/refs/heads/main/authentication/appnexus-authentication.yml
summary_line: token · 2 schemes
tags:
- Company
- Adtech
- Advertising
- Programmatic
- Ad Exchange
- DSP
- SSP
- Mobile SDK
- Marketing
---
