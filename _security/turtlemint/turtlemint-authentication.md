---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Turtlemint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turtlemint secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Turtlemint
provider_slug: turtlemint
scheme_count: 1
schemes:
- format: Bearer <access_token>
  header: Authorization
  in: header
  issued_via: Auth API (key + secret exchanged for a TTL-bound access token)
  name: AccessToken
  scheme: bearer
  sources:
  - https://developers.turtlefin.com/docs/type
  ttl: configurable per client
  type: http
slug: turtlemint-authentication
source_filename: turtlemint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.turtlefin.com/docs/type\ndocs: https://developers.turtlefin.com/docs/type\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_model: access-token\n  note: >-\n    Turtlefin OneAPI uses token-based authentication. Developers obtain an API\n    Key and Secret from the Apps section of the Developer Portal, then call the\n    Auth API to issue a short-lived Bearer Access Token (configurable TTL). The\n    token is passed in the Authorization header on every subsequent API call.\nschemes:\n  - name: AccessToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Bearer <access_token>\"\n    issued_via: Auth API (key + secret exchanged for a TTL-bound access token)\n    ttl: configurable per client\n    sources: [https://developers.turtlefin.com/docs/type]\ncredentials:\n  - name: API Key & Secret\n    obtained_from: Developer Portal > Apps section (https://app.turtlefin.com/dev-portal/login)\n\
  \    used_as: username/password to Authorize in the API docs and to call the Auth API\ntransport_security:\n  tls: required (SSL enabled; \"Data Security on Transit\")\nexample_request: |\n  curl 'https://app.turtlefin.com/api/minterprise/v1/products/private-car/lookups/rto?search=mh01' \\\n    --header 'Authorization: Bearer [YOUR_AUTH_INFO]' \\\n    --header 'Accept: application/json'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turtlemint/refs/heads/main/authentication/turtlemint-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Insurance Distribution
- Fintech
- API
- Payments
---
