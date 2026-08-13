---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Atmosplay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atmosplay declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Atmosplay
provider_slug: atmosplay
scheme_count: 0
schemes: []
slug: atmosplay-authentication
source_filename: atmosplay-authentication.yml
source_heading: Authentication Profile
source_url:
  status: 200
  url: https://github.com/Atmosplay/AtmosplayAds-Android/wiki/GetStarted
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://github.com/Atmosplay/AtmosplayAds-Android/wiki/GetStarted\nsources:\n  - url: https://github.com/Atmosplay/AtmosplayAds-Android/wiki/GetStarted\n    status: 200\n  - url: https://github.com/Atmosplay/AtmosplayAds-iOS\n    status: 200\n  - url: https://github.com/Atmosplay/Help-Center-for-Publisher/blob/master/guides.md\n    status: 200\n    note: publisher dashboard guide, sections 1.5 and 3.2\nderived_from_openapi: false\nnote: >-\n  DERIVED FROM PUBLISHED DOCS, NOT FROM A SPEC. Atmosplay published no OpenAPI and no\n  securitySchemes, so this profile is assembled from the credential model its own\n  integration docs describe. Two distinct surfaces existed; only the first is publicly\n  documented in any detail.\nsurfaces:\n  - name: AtmosplayAds mobile SDK\n    type: sdk-identifier-pair\n    status: documented\n    scheme: application-identifier\n    credentials:\n      - name: APP_ID\n        format: uppercase UUID\
  \ (8-4-4-4-12)\n        issued_by: Atmosplay publisher dashboard (\"Apps\" tab)\n        transport: passed to the SDK initializer in application code\n      - name: AD_UNIT_ID\n        format: uppercase UUID (8-4-4-4-12)\n        issued_by: Atmosplay publisher dashboard (\"AdUnits\" tab)\n        transport: passed to the ad-object constructor in application code\n    secret: false\n    rotation: not documented\n    note: >-\n      This is an identification pair, not an authentication secret — the values ship\n      inside a distributed mobile binary and are recoverable from it. Atmosplay published\n      public TEST values for both (see sandbox/). A wrong or unmatched pair surfaces as\n      SDK error 1002 \"request parameters error\" (see errors/).\n  - name: Atmosplay Report API\n    type: rest\n    status: gated-and-offline\n    scheme: api-key-plus-signature\n    credentials:\n      - name: Report API parameters\n        issued_by: >-\n          The Atmosplay publisher dashboard, \"\
  Setting\" tab (Chinese manual: 面板\"个人信息\"处)\n        transport: not publicly documented\n    reference_location: >-\n      Inside the authenticated dashboard only — the Chinese manual says the integration\n      doc was reachable via the dashboard's \"帮助文档\" (Help Docs) link. It was never\n      published to a public URL.\n    evidence:\n      - quote: >-\n          \"We support Report API for you to acquire data from interface. You can look up\n          your Report API in the 'Setting' tab on the dashboard.\"\n        url: https://github.com/Atmosplay/Help-Center-for-Publisher/blob/master/guides.md\n        status: 200\n      - quote: >-\n          \"我们提供Report API接口供您通过接口获取数据，Report API参数可在面板\"个人信息\"处获取，可点击\"帮助文档\"查看Report API对接文档\"\n        url: https://github.com/Atmosplay/Help-Center-for-Publisher/blob/master/系统使用手册.md\n        status: 200\n    note: >-\n      Atmosplay's own publisher guide confirms a Report API EXISTED, but the reference and\n      the credentials both lived behind\
  \ the dashboard login. The dashboard is gone —\n      atmosplay.com is a HugeDomains parking page — so the auth model, base URL, endpoints\n      and scopes are unrecoverable from any public surface. Nothing about this surface is\n      reconstructed or guessed here.\noauth: false\noauth_scopes: false\nmtls: false\nopenid_connect: false\ngaps:\n  - No OAuth 2.0, OpenID Connect, or scope surface was ever published — scopes/ is correctly absent.\n  - No key-rotation, key-prefix, or credential-lifecycle policy was published.\n  - >-\n    A Report API for the ACQUIRER, ZPLAY Ads, is publicly documented at\n    github.com/zplayads/report_api (hosts pa-report.zplayads.com and\n    pa-report-en.zplayads.com, API key + sha1 signature over key/timestamp/nonce). It is\n    ZPLAY's contract, on ZPLAY's hosts, describing the ZPLAY dashboard — NOT Atmosplay's —\n    and is deliberately not adopted here. See lifecycle/ for the successor lead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmosplay/refs/heads/main/authentication/atmosplay-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- AdTech
- Mobile
- Playable Ads
- Ad Monetization
- Gaming
- SDK
---
