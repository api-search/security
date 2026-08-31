---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Hungrypanda Authentication
name_suffix: Authentication
oauth_flows: []
overview: HungryPanda declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: HungryPanda
provider_slug: hungrypanda
scheme_count: 0
schemes: []
slug: hungrypanda-authentication
source_filename: hungrypanda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://www.redcatht.com/helpcentre/hungry-panda-integration-overview\nnote: 'HungryPanda publishes no developer portal and no authentication reference of its own. The\n  credential model below is stated by a first-party POS integrator''s public integration\n  documentation (Redcat) and corroborated by a live unauthenticated probe of the API host, which\n  rejects every request with a single envelope. No security scheme could be derived from a\n  specification because no specification is published.'\napis:\n- name: HungryPanda Merchant & Partner API\n  baseURL: https://api-uk-f2e.hungrypanda.co\n  schemes:\n  - id: partner-app-key\n    type: apiKey\n    confidence: medium\n    credentials:\n    - name: App Key\n      role: partner/application identifier\n    - name: Secret Key\n      role: shared secret used to authenticate the request\n    - name: ShopID\n      role: external store identifier scoping the credential to one\
  \ merchant location\n    issuance: 'Issued by HungryPanda to an approved merchant or POS partner. Redcat''s public\n      integration page states these three values \"must be obtained from Hungry Panda\".'\n    self_service: false\n    docs: https://www.redcatht.com/helpcentre/hungry-panda-integration-overview\n    note: 'The presence of a separate Secret Key alongside an App Key is the signature of a\n      request-signing scheme rather than a bearer key, but HungryPanda publishes no signing\n      algorithm, canonical-string format or header name, so the exact mechanism is NOT recorded\n      here. Do not assume HMAC.'\n  observed:\n    probe:\n      url: https://api-uk-f2e.hungrypanda.co/api/merchant/getCaptchagImage\n      method: GET\n      http_status: 200\n      body: '{\"code\":40001}'\n      probed: '2026-08-22'\n    behaviour: 'Every unauthenticated request — including /.well-known/*, /openapi.json and\n      /graphql — returns HTTP 200 with the same JSON body. The API signals\
  \ authentication failure\n      in the payload, not the status line, which means a client cannot distinguish \"not\n      authenticated\" from \"not found\" without parsing the body.'\n    cors: 'Access-Control-Allow-Origin: * with Access-Control-Allow-Credentials: true observed on\n      the response.'\n    edge: Cloudflare (cf-ray, __cf_bm cookie set for domain hungrypanda.co)\n  oauth2: false\n  openid_connect: false\n  mutual_tls: unknown\n  scopes: 'Not applicable — no OAuth surface exists, so no scopes/ artifact is emitted.'\ngaps:\n- 'No public authentication documentation on any hungrypanda.co host.'\n- 'No /.well-known/openid-configuration or /.well-known/oauth-authorization-server (both 404 on www; SPA/gateway shells elsewhere).'\n- 'Authentication failure is returned as HTTP 200 with an in-body code, defeating standard HTTP client error handling.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hungrypanda/refs/heads/main/authentication/hungrypanda-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Food Delivery
- Delivery
- Marketplace
- Restaurant
- Grocery
- Logistics
- E-Commerce
- Merchants
- Point-of-Sale
---
