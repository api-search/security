---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sendowl Authentication
name_suffix: Authentication
oauth_flows: []
overview: SendOwl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SendOwl
provider_slug: sendowl
scheme_count: 1
schemes:
- credential:
    enabled_by_default: false
    enablement: '"By default the API is not enabled on accounts so you must navigate to the Settings section, click the API link in the Advanced section and follow onscreen instructions to set this up."'
    password: API secret
    provisioning_url: https://dashboard.sendowl.com/settings/api_credentials
    username: API key
  description: '"In order for API calls to be accepted they must be sent with authorisation information. Specifically, an API key and secret must be passed through via Basic Auth." The API key is the Basic-Auth username and the API secret is the password, sent on the Authorization header.'
  example_documented: 'curl -H "Accept: text/xml" https://KEY:SECRET@api.sendowl.com/api/v1/products'
  name: basicAuth
  scheme: basic
  sources:
  - https://dashboard.sendowl.com/developers/api/introduction
  - https://help.sendowl.com/help/using-the-api
  type: http
slug: sendowl-authentication
source_filename: sendowl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://dashboard.sendowl.com/developers/api/introduction\ndocs: https://help.sendowl.com/help/using-the-api\nnote: >-\n  Derived-from-OpenAPI was not possible — SendOwl publishes no OpenAPI/Swagger document (see\n  conformance/sendowl-conformance.yml). This profile is read directly from the provider's own API\n  reference and help-center auth article.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    \"In order for API calls to be accepted they must be sent with authorisation information.\n    Specifically, an API key and secret must be passed through via Basic Auth.\" The API key is the\n    Basic-Auth username and the API secret is the password, sent on the Authorization header.\n  credential:\n    username: API key\n    password: API secret\n    provisioning_url:\
  \ https://dashboard.sendowl.com/settings/api_credentials\n    enabled_by_default: false\n    enablement: >-\n      \"By default the API is not enabled on accounts so you must navigate to the Settings section,\n      click the API link in the Advanced section and follow onscreen instructions to set this up.\"\n  example_documented: 'curl -H \"Accept: text/xml\" https://KEY:SECRET@api.sendowl.com/api/v1/products'\n  sources:\n  - https://dashboard.sendowl.com/developers/api/introduction\n  - https://help.sendowl.com/help/using-the-api\npermissions:\n  model: per-key permission checkboxes assigned at key creation\n  documented: >-\n    \"When creating API keys, you'll be prompted to assign permissions... In most cases, it's best to\n    click the Manager checkbox for full permissions.\"\n  named_roles:\n  - Manager\n  note: >-\n    SendOwl publishes no enumerated scope/permission reference, so the full set of checkboxes is not\n    machine-readable. There is no OAuth surface and therefore\
  \ no scopes/ artifact for this provider.\n  source: https://help.sendowl.com/help/using-the-api\ntransport:\n  https_required: false\n  documented: >-\n    \"Although not required, it is highly recommended to send requests over HTTPS due to the nature of\n    the information and the fact that the API key and secret will be sent in plaintext otherwise.\"\n  note: >-\n    HTTPS is recommended rather than enforced in the documentation; the credential is a long-lived\n    static key/secret pair with no rotation or expiry contract published.\nwebhook_authentication:\n  direction: inbound-to-subscriber\n  header: X-SENDOWL-HMAC-SHA256\n  algorithm: HMAC-SHA256, base64-encoded\n  key: The Signing Key Secret from the SendOwl API settings page\n  payload: The raw request JSON body\n  source: https://help.sendowl.com/help/using-web-hooks\nguidance:\n  credential_exposure: >-\n    SendOwl explicitly warns against embedding API credentials in distributed software: \"Do not include\n    calls to this\
  \ API endpoint in your software... this will expose your API key and secret to anyone\n    examining your source code or watching wire data.\" License validation should be proxied through the\n    seller's own server.\n  source: https://dashboard.sendowl.com/developers/api/licenses\nx-evidence:\n- url: https://dashboard.sendowl.com/developers/api/introduction\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://help.sendowl.com/help/using-the-api\n  http_status: 200\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendowl/refs/heads/main/authentication/sendowl-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- E-Commerce
- Digital Products
- Payments
- Subscriptions
- Checkout
- Memberships
- Licensing
- Creator Economy
- Webhooks
---
