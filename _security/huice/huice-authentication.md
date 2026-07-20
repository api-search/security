---
api_key_in:
- query
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Huice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huice secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Huice
provider_slug: huice
scheme_count: 1
schemes:
- example_concatenation: 06-appkey:0008-test2-xx;08-end_time:0019-2016-08-01 13:00:00
  in: request-parameters
  name: WangdiantongSignature
  parameters:
  - description: Seller account identifier assigned by Wangdiantong.
    name: sid
    required: true
  - description: Interface (integration) account created in the self-service integration module.
    name: appkey
    required: true
  - description: Beijing time as a 10-digit Unix epoch seconds value.
    name: timestamp
    required: true
  - description: 32-bit lowercase MD5 signature of the request parameters (see signature below).
    name: sign
    required: true
  secret:
    description: Shared secret paired with appkey; used only to compute sign, never sent on the wire.
    name: appsecret
    transmitted: false
  signature:
    algorithm: MD5
    docs: https://open.wangdian.cn/open/guide?path=guide_signsf
    output: 32-bit lowercase hex
    steps:
    - Include all request parameters except appsecret.
    - Sort parameters by key name in ascending order.
    - For each pair, prefix the key with its 2-digit key-length and a '-'; prefix the value with its 4-digit value-length (or the actual length when it exceeds 4 digits) and a '-'; join key and value parts with ':'; terminate each parameter with ';' (except the last).
    - Append appsecret directly to the end of the concatenated string (no separator).
    - Compute the 32-bit lowercase MD5 of that string; the result is the sign parameter.
  type: signature
slug: huice-authentication
source_filename: huice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://open.wangdian.cn/open/guide?path=guide_signsf\ndocs: https://open.wangdian.cn/open/guide?path=guide_kfzn\nsummary:\n  types:\n  - signature\n  api_key_in:\n  - query\n  oauth2_flows: []\n  note: >-\n    Wangdiantong Open Platform uses a custom request-signature scheme (sid + appkey + timestamp +\n    sign). It is not OAuth2/OIDC and not a simple static bearer key; the shared appsecret is never\n    transmitted and is used only to compute the sign.\nschemes:\n- name: WangdiantongSignature\n  type: signature\n  in: request-parameters\n  parameters:\n  - name: sid\n    required: true\n    description: Seller account identifier assigned by Wangdiantong.\n  - name: appkey\n    required: true\n    description: Interface (integration) account created in the self-service integration module.\n  - name: timestamp\n    required: true\n    description: Beijing time as a 10-digit Unix epoch seconds value.\n  - name: sign\n    required:\
  \ true\n    description: 32-bit lowercase MD5 signature of the request parameters (see signature below).\n  secret:\n    name: appsecret\n    transmitted: false\n    description: Shared secret paired with appkey; used only to compute sign, never sent on the wire.\n  signature:\n    algorithm: MD5\n    output: 32-bit lowercase hex\n    docs: https://open.wangdian.cn/open/guide?path=guide_signsf\n    steps:\n    - Include all request parameters except appsecret.\n    - Sort parameters by key name in ascending order.\n    - For each pair, prefix the key with its 2-digit key-length and a '-'; prefix the value with its\n      4-digit value-length (or the actual length when it exceeds 4 digits) and a '-'; join key and\n      value parts with ':'; terminate each parameter with ';' (except the last).\n    - Append appsecret directly to the end of the concatenated string (no separator).\n    - Compute the 32-bit lowercase MD5 of that string; the result is the sign parameter.\n  example_concatenation:\
  \ '06-appkey:0008-test2-xx;08-end_time:0019-2016-08-01 13:00:00'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huice/refs/heads/main/authentication/huice-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- Enterprise
- E-commerce
- ERP
- Order Management
- Inventory Management
- Warehouse Management
- Retail
- SaaS
- China
---
