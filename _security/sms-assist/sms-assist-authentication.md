---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sms Assist Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SMS Assist secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SMS Assist
provider_slug: sms-assist
scheme_count: 2
schemes:
- description: HTTP Basic Auth (username + password) presented to the environment /token endpoint to obtain an access_token. Client and Vendor surfaces have separate credentials and separate token endpoints.
  name: BasicAuthTokenExchange
  scheme: basic
  token_endpoints:
    client:
      dev: https://meshdev.lessen.com/one-graph-client/token
      production: https://meshlive.lessen.com/one-graph-client/token
      stage: https://meshstage.lessen.com/one-graph-client/token
    vendor:
      production: https://meshlive.lessen.com/one-graph-vendor/token
      stage: https://meshstage.lessen.com/one-graph-vendor/token
  type: http
- bearerFormat: access_token
  description: Bearer access_token returned by the /token endpoint, sent on every GraphQL request. Expires after the period given by the response `expires_in` property (Unix epoch time); regenerate by repeating the Basic Auth exchange.
  name: BearerToken
  scheme: bearer
  type: http
slug: sms-assist-authentication
source_filename: sms-assist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.lessen.com/docs/#/client/authentication/client\ndocs:\n- https://developers.lessen.com/docs/#/client/authentication/client\n- https://developers.lessen.com/docs/#/vendor/authentication/vendor\nsummary:\n  types: [http, oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  model: >-\n    Token-based (bearer) authentication. Callers exchange HTTP Basic Auth\n    credentials (client-specific username/password issued per developer account\n    and environment) at a /token endpoint for a short-lived bearer access_token,\n    then send that token on every GraphQL request. Documentation notes OAuth 2.0\n    is the underlying protocol. Unauthorized calls return 401.\nschemes:\n- name: BasicAuthTokenExchange\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic Auth (username + password) presented to the environment /token\n    endpoint to obtain an access_token. Client and Vendor surfaces\
  \ have separate\n    credentials and separate token endpoints.\n  token_endpoints:\n    client:\n      stage: https://meshstage.lessen.com/one-graph-client/token\n      dev: https://meshdev.lessen.com/one-graph-client/token\n      production: https://meshlive.lessen.com/one-graph-client/token\n    vendor:\n      stage: https://meshstage.lessen.com/one-graph-vendor/token\n      production: https://meshlive.lessen.com/one-graph-vendor/token\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: access_token\n  description: >-\n    Bearer access_token returned by the /token endpoint, sent on every GraphQL\n    request. Expires after the period given by the response `expires_in`\n    property (Unix epoch time); regenerate by repeating the Basic Auth exchange.\nwebhook_auth:\n  description: >-\n    Outbound webhook deliveries are secured per subscription with an Application\n    Id and a shared Secret (HMAC signing key), and optionally JWT Bearer Token\n    authentication against\
  \ the subscriber's endpoint (added Oct 2025). Custom\n    header injection and per-endpoint test-connection validation are supported.\nsso:\n  description: >-\n    Client Portal and Resident Portal support SSO and SCIM 2.0 user\n    provisioning. Documented identity providers: Okta, OneLogin, and Azure AD.\n  docs: https://developers.lessen.com/docs/#/client/sso/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sms-assist/refs/heads/main/authentication/sms-assist-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Facilities Management
- Property Maintenance
- Work Orders
- Field Service
- Maintenance
- Real Estate
- GraphQL
- Webhooks
- Vendor Network
---
