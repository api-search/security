---
anonymous_access: false
api_key_in: []
api_specs:
- filename: steadyapi-collection.json
  format: json
  label: SteadyAPI
  slug: steadyapi
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/steadyapi/refs/heads/main/postman/steadyapi-collection.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Steadyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SteadyAPI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SteadyAPI
provider_slug: steadyapi
scheme_count: 2
schemes:
- description: Send the personal access token as an Authorization header with the value "Bearer {YOUR_AUTH_KEY}". Endpoints requiring auth are marked with a "requires authentication" badge in the documentation.
  in: header
  name: Authorization
  scheme: bearer
  type: http
- description: 'Alternative browser-friendly authentication: pass the personal access token as an "apikey" query parameter, e.g. https://api.steadyapi.com/v1/markets/search?search=AA&apikey={YOUR_AUTH_KEY}'
  in: query
  name: apikey
  type: apiKey
slug: steadyapi-authentication
source_filename: steadyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: searched\nsource: https://docs.steadyapi.com\ndocs: https://docs.steadyapi.com\nsummary: >-\n  SteadyAPI authenticates every protected endpoint with a personal access token.\n  The token is sent either as an HTTP Authorization header (\"Bearer {YOUR_AUTH_KEY}\")\n  or, for browser/GET use, as an \"apikey\" query-string parameter. Tokens are\n  generated and revoked by the account holder from the dashboard (Account ->\n  Personal Access Tokens). No OAuth 2.0 / OpenID Connect flow is documented.\nschemes:\n- type: http\n  scheme: bearer\n  name: Authorization\n  in: header\n  description: >-\n    Send the personal access token as an Authorization header with the value\n    \"Bearer {YOUR_AUTH_KEY}\". Endpoints requiring auth are marked with a\n    \"requires authentication\" badge in the documentation.\n- type: apiKey\n  name: apikey\n  in: query\n  description: >-\n    Alternative browser-friendly authentication: pass the personal access token\n\
  \    as an \"apikey\" query parameter, e.g.\n    https://api.steadyapi.com/v1/markets/search?search=AA&apikey={YOUR_AUTH_KEY}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadyapi/refs/heads/main/authentication/steadyapi-authentication.yml
summary_line: 2 schemes
tags:
- Data
- Finance
- Stock Market
- Social Media
- Reddit
- Data as a Service
- Web Data
- Alternative Data
---
