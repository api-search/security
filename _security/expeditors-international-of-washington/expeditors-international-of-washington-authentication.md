---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Expeditors International Of Washington Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Expeditors International of Washington secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Expeditors International of Washington
provider_slug: expeditors-international-of-washington
scheme_count: 3
schemes:
- applies_to: POST /oauth2/token
  description: 'The token endpoint is authenticated with HTTP Basic: the Base64 encoding of clientId:clientSecret in an `Authorization: Basic {clientCredentials}` header. Client id and secret are issued by Expeditors when a customer application is registered.'
  name: TokenRequestBasic
  scheme: basic
  sources:
  - https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm
  type: http
- description: POST grant_type=client_credentials (form-urlencoded) to the token endpoint. No other grant type is accepted. The response carries access_token, token_type "bearer", expires_in and scope "application".
  flow: clientCredentials
  grant_types:
  - client_credentials
  name: OAuth2ClientCredentials
  scopes:
  - application
  sources:
  - https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm
  token_lifetime_seconds: 900
  token_type: bearer
  token_url: https://api.expeditors.com/tracking/v2/oauth2/token
  type: oauth2
- applies_to: all resource endpoints under /tracking/v2
  description: 'All resource requests carry `Authorization: Bearer {token}`.'
  name: BearerToken
  scheme: bearer
  sources:
  - https://help.expeditors.com/globalhelp/shipment_api/get_shipments.htm
  type: http
slug: expeditors-international-of-washington-authentication
source_filename: expeditors-international-of-washington-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm\ndocs: https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm\nnote: >-\n  Expeditors publishes no OpenAPI, so this profile is read from the API\n  Developer Center documentation rather than derived from securitySchemes.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: TokenRequestBasic\n    type: http\n    scheme: basic\n    applies_to: POST /oauth2/token\n    description: >-\n      The token endpoint is authenticated with HTTP Basic: the Base64 encoding\n      of clientId:clientSecret in an `Authorization: Basic {clientCredentials}`\n      header. Client id and secret are issued by Expeditors when a customer\n      application is registered.\n    sources: [https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm]\n  - name: OAuth2ClientCredentials\n   \
  \ type: oauth2\n    flow: clientCredentials\n    token_url: https://api.expeditors.com/tracking/v2/oauth2/token\n    grant_types: [client_credentials]\n    scopes: [application]\n    token_type: bearer\n    token_lifetime_seconds: 900\n    description: >-\n      POST grant_type=client_credentials (form-urlencoded) to the token\n      endpoint. No other grant type is accepted. The response carries\n      access_token, token_type \"bearer\", expires_in and scope \"application\".\n    sources: [https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm]\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    applies_to: all resource endpoints under /tracking/v2\n    description: 'All resource requests carry `Authorization: Bearer {token}`.'\n    sources: [https://help.expeditors.com/globalhelp/shipment_api/get_shipments.htm]\noperational_notes:\n  - Multiple tokens may be active simultaneously; requesting a new token does not revoke earlier ones.\n  - Separate development\
  \ and production credential sets are available on request from an Expeditors representative.\n  - Tokens can expire early in edge cases; the documented pattern is to reuse a token until a call returns invalid_token, then re-request and replay.\n  - The token endpoint is separately rate limited to 10 requests per hour.\nregistration:\n  self_service: false\n  process: Contact an Expeditors representative with organization name plus business and technical contact names/emails.\n  url: https://help.expeditors.com/globalhelp/shipment_api/getting_started.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expeditors-international-of-washington/refs/heads/main/authentication/expeditors-international-of-washington-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Customs
- Freight Forwarding
- Logistics
- Supply Chain
- Warehousing
- Shipment Tracking
- Transportation
- Order Management
- Customs Brokerage
- Visibility
---
