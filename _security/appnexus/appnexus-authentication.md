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
overview: AppNexus secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppNexus
provider_slug: appnexus
scheme_count: 1
schemes:
- carry:
  - 'Authorization: <TOKEN> request header'
  - session cookie (curl -b cookies -c cookies)
  error_signal: error_id NOAUTH in response envelope signals re-authentication needed
  jwt_option: https://learn.microsoft.com/xandr/digital-platform-api/token-based-api-authentication
  mechanism: username-password-token-exchange
  name: token
  obtain: POST https://api.appnexus.com/auth with JSON body {auth:{username,password}}; returns response.token
  reauth_limit: 10 successful auths per 5-minute period
  token_lifetime: 2 hours idle; 24-hour hard expiry regardless of activity
  type: token
slug: appnexus-authentication
source_filename: appnexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://learn.microsoft.com/xandr/digital-platform-api/authentication-service\ndocs: https://learn.microsoft.com/xandr/digital-platform-api/authentication-service\nsummary:\n  types: [token]\n  scheme: custom-token\n  oauth2: false\n  api_key_in: [header, cookie]\nschemes:\n  - name: token\n    type: token\n    mechanism: username-password-token-exchange\n    obtain: \"POST https://api.appnexus.com/auth with JSON body {auth:{username,password}}; returns response.token\"\n    carry:\n      - \"Authorization: <TOKEN> request header\"\n      - \"session cookie (curl -b cookies -c cookies)\"\n    token_lifetime: \"2 hours idle; 24-hour hard expiry regardless of activity\"\n    reauth_limit: \"10 successful auths per 5-minute period\"\n    jwt_option: https://learn.microsoft.com/xandr/digital-platform-api/token-based-api-authentication\n    error_signal: \"error_id NOAUTH in response envelope signals re-authentication needed\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appnexus/refs/heads/main/authentication/appnexus-authentication.yml
summary_line: token · 1 scheme
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
