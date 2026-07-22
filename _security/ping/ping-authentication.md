---
api_key_in:
- basic-auth-username
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ping Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ping++ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ping++
provider_slug: ping
scheme_count: 1
schemes:
- description: Ping++ API uses HTTP Basic authentication. The merchant API Key is supplied as the Basic-auth username; the password is left empty. All requests must be sent over HTTPS — plain HTTP is rejected by the Ping++ servers. The API Key is managed in the merchant dashboard under 企业面板 → 开发参数.
  example: 'curl https://api.pingxx.com/v1/charges -u sk_test_XXXXXXXXXXXXXXXXXXXXXXXX:'
  key_prefixes:
    live: sk_live_
    test: sk_test_
  modes:
  - description: Real transaction environment (真实交易环境).
    mode: live
  - description: Test environment (模拟测试交易环境). Test-mode keys simulate transactions and webhooks without any real money movement or fees; live and test modes can be switched in real time.
    mode: test
  name: ApiKeyBasicAuth
  scheme: http-basic
  type: apiKey
slug: ping-authentication
source_filename: ping-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pingxx.com/api/%E8%AE%A4%E8%AF%81.html\ndocs: https://docs.pingxx.com/api/\nsummary:\n  types: [apiKey]\n  scheme: http-basic\n  api_key_in: [basic-auth-username]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyBasicAuth\n  type: apiKey\n  scheme: http-basic\n  description: >-\n    Ping++ API uses HTTP Basic authentication. The merchant API Key is supplied as the\n    Basic-auth username; the password is left empty. All requests must be sent over HTTPS —\n    plain HTTP is rejected by the Ping++ servers. The API Key is managed in the merchant\n    dashboard under 企业面板 → 开发参数.\n  key_prefixes:\n    live: sk_live_\n    test: sk_test_\n  modes:\n    - mode: live\n      description: Real transaction environment (真实交易环境).\n    - mode: test\n      description: >-\n        Test environment (模拟测试交易环境). Test-mode keys simulate transactions and webhooks\n        without any real money movement or fees; live and test modes can\
  \ be switched in real time.\n  example: 'curl https://api.pingxx.com/v1/charges -u sk_test_XXXXXXXXXXXXXXXXXXXXXXXX:'\nnotes: >-\n  Ping++ does not use OAuth or OpenID Connect — there is no scope surface, so no scopes/ artifact\n  is emitted. Authorization is coarse-grained via the merchant API Key. Multi-tier merchant setups\n  scope calls to a sub-merchant via the app[id] request parameter rather than a distinct credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ping/refs/heads/main/authentication/ping-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Aggregated Payment
- 聚合支付
- FinTech
- Payment Gateway
- Split Settlement
- WeChat Pay
- Alipay
- UnionPay
- China
- Payouts
---
