---
api_key_in:
- body
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aci Worldwide Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACI Worldwide secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ACI Worldwide
provider_slug: aci-worldwide
scheme_count: 2
schemes:
- description: 'Authorization Bearer header carrying the access token issued per merchant/ channel. Retrieved from the backend portal under Administration > Account data > Merchant / Channel Info. Sent as `Authorization: Bearer <token>`.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.aciworldwide.com/reference/parameters
  type: http
- description: The entity required to authorize the request. This should be the channel entity identifier. If channel dispatching is activated it should be the merchant entity identifier. Sent as a body parameter alongside the bearer token (for HTTP POST all parameters must be in the message body, not the URL).
  format: AN32
  in: body
  name: entityId
  parameter: entityId
  required: conditional
  sources:
  - https://docs.aciworldwide.com/reference/parameters
  type: apiKey
slug: aci-worldwide-authentication
source_filename: aci-worldwide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://docs.aciworldwide.com/reference/parameters\ndocs: https://docs.aciworldwide.com/reference/parameters\nsummary:\n  types: [http, apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\n  note: >-\n    The ACI Open Payment Platform (PAY.ON / oppwa gateway) authenticates every\n    request with an HTTP Authorization Bearer access token, scoped to a channel\n    by a required entityId parameter carried in the request body. There is no\n    OAuth2 authorization/token endpoint and no OpenAPI security scheme published;\n    this profile is captured from the documented request parameters.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Authorization Bearer header carrying the access token issued per merchant/\n      channel. Retrieved from the backend portal under Administration > Account\n      data > Merchant / Channel Info. Sent as `Authorization: Bearer <token>`.\n    in: header\n\
  \    parameter: Authorization\n    sources: [https://docs.aciworldwide.com/reference/parameters]\n  - name: entityId\n    type: apiKey\n    in: body\n    parameter: entityId\n    format: AN32\n    required: conditional\n    description: >-\n      The entity required to authorize the request. This should be the channel\n      entity identifier. If channel dispatching is activated it should be the\n      merchant entity identifier. Sent as a body parameter alongside the bearer\n      token (for HTTP POST all parameters must be in the message body, not the URL).\n    sources: [https://docs.aciworldwide.com/reference/parameters]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aci-worldwide/refs/heads/main/authentication/aci-worldwide-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Payments
- United States
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- eCommerce
- Fraud
- Tokenization
- 3D Secure
- Bill Payment
- Real-Time Payments
- ISO 20022
---
