---
api_key_in:
- sdk-configuration
auth_types:
- apiKey
- cookie
description: ''
kind: authentication
layout: security
method: searched
name: Qeenai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qeen.AI secures its APIs with apiKey and cookie across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qeen.AI
provider_slug: qeenai
scheme_count: 3
schemes:
- in: sdk-configuration
  key_prefix: null
  key_prefix_note: not published
  name: MobileSDKApiKey
  note: The key is paired with a customer-provisioned `host` — the SDK has no default ingestion endpoint. The compiled framework binary names only PostHog's own asset hosts (us.i.posthog.com, eu.i.posthog.com and their asset siblings), consistent with the README's statement that PostHog is "baked INTO the framework and hidden"; the customer's `host` is the PostHog-compatible ingestion endpoint Qeen provisions for that account.
  parameter: apiKey
  rotation: not documented
  signature: 'QeenSDK.configure(apiKey: String, host: String, debug: Bool = false, options: [String: Any] = [:])'
  sources:
  - packages/qeenai-ios-sdk-interface.swiftinterface
  surface: Qeen Mobile Analytics SDK (iOS + Android)
  type: apiKey
- in: script-url
  name: WebSDKProjectBinding
  note: The browser loader carries no secret. It derives a 7-character non-cryptographic hash (a djb2-style rolling hash, base-32, zero-padded) of the page URL and of a device id persisted in localStorage under "fodoole_uid", and requests the content-replacement script at fodoole-web-analytics-qfan6cresq-ew.a.run.app/qeen-script/{hash}. Project and website identity (projectId, websiteId, contentServingId) then arrive from the server in the client config rather than being embedded in the page. This is site-binding, not authentication — there is no bearer credential on the browser data plane.
  parameter: 'path segment: /qeen-script/{hash(pageUrl)}{hash(userDeviceId)}'
  sources:
  - https://cdn.qeen.ai/loader/main.js
  - https://cdn.qeen.ai/sdk/qeen.js
  surface: Qeen Web SDK loader (https://cdn.qeen.ai/loader/main.js)
  type: apiKey
- evidence:
  - body: '{"detail":"Authentication credentials were not provided."}'
    status: 401
    url: https://users.qeen.ai/api/v1/core/websites
  - body: '{"detail":"Authentication credentials were not provided."}'
    status: 401
    url: https://users.qeen.ai/api/v1/subscriptions/products
  - body: '{"valid":false,"message":"... Token is required. ..."}'
    status: 400
    url: https://users.qeen.ai/api/v1/auth/verify-token/
  - body: '{"detail":"Method \"GET\" not allowed."}'
    method: GET
    status: 405
    url: https://users.qeen.ai/api/v1/auth/verify-token/
  framework: Django REST Framework
  in: cookie
  name: CustomerPlatformSession
  note: The customer web application (app.qeen.ai, a Nuxt SPA) calls its backend at users.qeen.ai with credentials:"include". Token lifecycle endpoints are POST /api/v1/auth/verify-token/ and POST /api/v1/auth/refresh-token/. Unauthenticated requests to business endpoints return DRF's standard 401 body {"detail":"Authentication credentials were not provided."}. This is the product's own session surface, not a developer API — no key issuance, no scopes, no public documentation.
  sources:
  - live probe
  surface: https://users.qeen.ai/api/v1/
  type: cookie
slug: qeenai-authentication
source_filename: qeenai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://github.com/fodoole/qeen-mobile-sdk-ios (README + published .swiftinterface),\n  https://github.com/fodoole/qeen-maven (README), https://cdn.qeen.ai/sdk/qeen.js,\n  and live unauthenticated probes of https://users.qeen.ai/api/v1/* on 2026-08-12\ndocs: https://github.com/fodoole/qeen-mobile-sdk-ios#usage\nnote: >-\n  Qeen publishes no OpenAPI, so nothing here is derived from a spec. Every scheme below is read\n  from a first-party artifact the company distributes publicly (its SDK source, its SDK READMEs)\n  or observed on a live unauthenticated request. Credentials themselves are NOT self-serve:\n  both mobile READMEs state the host and API key \"are shared privately by email — contact\n  tech@qeen.ai\", so there is no public key-issuance flow to document.\n\nsummary:\n  types: [apiKey, cookie]\n  api_key_in: [sdk-configuration]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n\
  \  self_serve_credentials: false\n  credential_request_channel: tech@qeen.ai\n\nschemes:\n  - name: MobileSDKApiKey\n    type: apiKey\n    in: sdk-configuration\n    parameter: apiKey\n    surface: Qeen Mobile Analytics SDK (iOS + Android)\n    signature: 'QeenSDK.configure(apiKey: String, host: String, debug: Bool = false, options: [String: Any] = [:])'\n    sources: [packages/qeenai-ios-sdk-interface.swiftinterface]\n    note: >-\n      The key is paired with a customer-provisioned `host` — the SDK has no default ingestion\n      endpoint. The compiled framework binary names only PostHog's own asset hosts\n      (us.i.posthog.com, eu.i.posthog.com and their asset siblings), consistent with the README's\n      statement that PostHog is \"baked INTO the framework and hidden\"; the customer's `host` is\n      the PostHog-compatible ingestion endpoint Qeen provisions for that account.\n    key_prefix: null\n    key_prefix_note: not published\n    rotation: not documented\n\n  - name: WebSDKProjectBinding\n\
  \    type: apiKey\n    in: script-url\n    parameter: 'path segment: /qeen-script/{hash(pageUrl)}{hash(userDeviceId)}'\n    surface: Qeen Web SDK loader (https://cdn.qeen.ai/loader/main.js)\n    sources: [https://cdn.qeen.ai/loader/main.js, https://cdn.qeen.ai/sdk/qeen.js]\n    note: >-\n      The browser loader carries no secret. It derives a 7-character non-cryptographic hash (a\n      djb2-style rolling hash, base-32, zero-padded) of the page URL and of a device id persisted\n      in localStorage under \"fodoole_uid\", and requests the content-replacement script at\n      fodoole-web-analytics-qfan6cresq-ew.a.run.app/qeen-script/{hash}. Project and website\n      identity (projectId, websiteId, contentServingId) then arrive from the server in the client\n      config rather than being embedded in the page. This is site-binding, not authentication —\n      there is no bearer credential on the browser data plane.\n\n  - name: CustomerPlatformSession\n    type: cookie\n    in: cookie\n\
  \    surface: https://users.qeen.ai/api/v1/\n    framework: Django REST Framework\n    sources: [live probe]\n    note: >-\n      The customer web application (app.qeen.ai, a Nuxt SPA) calls its backend at users.qeen.ai\n      with credentials:\"include\". Token lifecycle endpoints are POST /api/v1/auth/verify-token/\n      and POST /api/v1/auth/refresh-token/. Unauthenticated requests to business endpoints return\n      DRF's standard 401 body {\"detail\":\"Authentication credentials were not provided.\"}. This is\n      the product's own session surface, not a developer API — no key issuance, no scopes, no\n      public documentation.\n    evidence:\n      - {url: 'https://users.qeen.ai/api/v1/core/websites', status: 401, body: '{\"detail\":\"Authentication credentials were not provided.\"}'}\n      - {url: 'https://users.qeen.ai/api/v1/subscriptions/products', status: 401, body: '{\"detail\":\"Authentication credentials were not provided.\"}'}\n      - {url: 'https://users.qeen.ai/api/v1/auth/verify-token/',\
  \ status: 400, body: '{\"valid\":false,\"message\":\"... Token is required. ...\"}'}\n      - {url: 'https://users.qeen.ai/api/v1/auth/verify-token/', method: GET, status: 405, body: '{\"detail\":\"Method \\\"GET\\\" not allowed.\"}'}\n\nunauthenticated_surfaces:\n  - url: https://fodoole-web-analytics-qfan6cresq-ew.a.run.app/search-results\n    status: 400\n    body: '{\"error\":\"Empty search query provided\"}'\n    note: >-\n      Answers anonymously and validates input rather than rejecting on auth — the embedded search\n      widget's backing endpoint takes no credential from the browser.\n  - url: https://fodoole-web-analytics-qfan6cresq-ew.a.run.app/sdk/client-config\n    status: 400\n    body: 'Unsupported URL'\n    note: Anonymous; requires site/page parameters the loader supplies.\n\nnot_found:\n  - oauth2 authorization server\n  - openid-connect discovery\n  - scoped access tokens\n  - public API key self-service / developer portal\n  - mTLS\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qeenai/refs/heads/main/authentication/qeenai-authentication.yml
summary_line: apiKey/cookie · 3 schemes
tags:
- Company
- Ai
- Marketing
- Ecommerce
- Advertising
- MENA
- Analytics
- Personalization
- Mobile SDK
- Content Optimization
- Search
- Attribution
---
