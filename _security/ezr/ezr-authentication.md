---
api_key_in:
- form-body
auth_types:
- signedRequest
description: ''
kind: authentication
layout: security
method: searched
name: Ezr Authentication
name_suffix: Authentication
oauth_flows: []
overview: EZR secures its APIs with signedRequest across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EZR
provider_slug: ezr
scheme_count: 1
schemes:
- credentials:
  - description: 品牌接入的应用编号/品牌编码 — the brand/merchant application code issued by EZR
    name: AppId
    required: true
    type: string
  - description: shared secret held by the client; never transmitted
    name: Token
    only mixed into the signature: null
    required: true
    type: string
  - ERP): null
    also the rate-limit key: null
    description: 对接系统来源 — the calling system identifier (e.g. POS
    name: AppSystem
    required: true
    type: string
  - description: yyyyMMddHHmmss; rejected with StatusCode 308 if more than 10 minutes out
    name: Timestamp
    required: true
    type: string
  - description: uppercase hex request signature
    name: Sign
    required: true
    type: string
  - description: business parameters as a JSON string
    name: Args
    required: true
    type: string
  in: form-body
  name: EZRSignedRequest
  response_verification:
    algorithm: SHA1 over the same AppId/Timestamp/Token canonical string
    field: Sign
    rule: Verify the response Sign before acting on Result; ignore the message entirely if verification fails. Do not verify when Status=false.
    signed: true
  signing:
    algorithm_alternate: MD5 (32) — must be enabled by the EZR project manager
    algorithm_default: SHA1
    canonical_string: AppId={AppId}&Timestamp={Timestamp}&Token={Token}
    canonicalisation: parameter names sorted in English dictionary order, joined as a query string, UTF-8 bytes
    encoding: hexadecimal, uppercase
    published_example:
      input: AppId=EZP&Timestamp=20150701093010&Token=9cd8c0ed38a9e113
      note: The provider's guide prints worked SHA1 and MD5 outputs for this input; they are illustrative doc values, not credentials, and are intentionally not reproduced here.
  transport: HTTPS POST, application/x-www-form-urlencoded, UTF-8
  type: signedRequest
  webhook_verification:
    applies_to: asyncapi/ezr-webhooks.yml
    note: EZR signs its outbound pushes with the same scheme, so receivers can verify inbound pushes.
slug: ezr-authentication
source_filename: ezr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://open.ezrpro.com/#/apiFile/guide/00001\ndocs: https://open.ezrpro.com/#/apiFile/guide/00003\nnote: >-\n  Derived from the EZR Open Platform developer guide (开发指南) and signing-algorithm page\n  (加签、验签算法), both published anonymously at open.ezrpro.com, and corroborated by the\n  provider's own packaged Agent Skill (skills/ezr-common-infrastructure.md). EZR publishes no\n  OpenAPI, so there are no OpenAPI securitySchemes to derive from — this profile is read from\n  the provider's prose reference, not fabricated.\nsummary:\n  types: [signedRequest]\n  oauth2: false\n  openid_connect: false\n  api_key_in: [form-body]\n  bearer: false\n  mutual_tls: false\n  scopes: none — access is granted per interface at provisioning time, not by scope\nonboarding:\n  steps:\n  - 申请商家代码AppID和接口请求地址 — request a brand/merchant AppId and the interface request address from EZR\n  - 开放平台会分配接入参数Token和Appsystem，并开通接口权限 — EZR issues the Token\
  \ and AppSystem and enables interface permissions\n  - 按照接口文档实现业务逻辑 — implement against the interface reference\n  self_service: false\n  gate: EZR technical support / account manager assigns credentials; there is no public sign-up\n  source: https://open.ezrpro.com/#/apiFile/guide/00001\nschemes:\n- name: EZRSignedRequest\n  type: signedRequest\n  in: form-body\n  transport: HTTPS POST, application/x-www-form-urlencoded, UTF-8\n  credentials:\n  - {name: AppId, type: string, required: true, description: 品牌接入的应用编号/品牌编码 — the brand/merchant application code issued by EZR}\n  - {name: Token, type: string, required: true, description: shared secret held by the client; never transmitted, only mixed into the signature}\n  - {name: AppSystem, type: string, required: true, description: 对接系统来源 — the calling system identifier (e.g. POS, ERP), also the rate-limit key}\n  - {name: Timestamp, type: string, required: true, description: 'yyyyMMddHHmmss; rejected with StatusCode 308 if more than 10 minutes\
  \ out'}\n  - {name: Sign, type: string, required: true, description: uppercase hex request signature}\n  - {name: Args, type: string, required: true, description: business parameters as a JSON string}\n  signing:\n    algorithm_default: SHA1\n    algorithm_alternate: MD5 (32) — must be enabled by the EZR project manager\n    canonical_string: AppId={AppId}&Timestamp={Timestamp}&Token={Token}\n    canonicalisation: parameter names sorted in English dictionary order, joined as a query string, UTF-8 bytes\n    encoding: hexadecimal, uppercase\n    published_example:\n      input: AppId=EZP&Timestamp=20150701093010&Token=9cd8c0ed38a9e113\n      note: >-\n        The provider's guide prints worked SHA1 and MD5 outputs for this input; they are\n        illustrative doc values, not credentials, and are intentionally not reproduced here.\n  response_verification:\n    signed: true\n    algorithm: SHA1 over the same AppId/Timestamp/Token canonical string\n    field: Sign\n    rule: >-\n      Verify\
  \ the response Sign before acting on Result; ignore the message entirely if\n      verification fails. Do not verify when Status=false.\n  webhook_verification:\n    applies_to: asyncapi/ezr-webhooks.yml\n    note: EZR signs its outbound pushes with the same scheme, so receivers can verify inbound pushes.\nnetwork_controls:\n- control: ip-allowlist\n  required: true\n  description: >-\n    Access is IP-restricted; a call from an unregistered address is rejected with StatusCode\n    400 (访问受限通常指不在IP白名单). Interfaces are enabled by default once granted, but\n    re-enabling requires configuring the IP address.\n  source: https://doc.ezrpro.com/ (help centre, per search result) and status code 400\nenvironments:\n- {name: 测试环境 (test), https: 'https://open-q1.ezrpro.com', http: null}\n- {name: UCloud, https: 'https://open-up.ezrpro.com', http: 'http://open-up.ezrpro.com'}\n- {name: QCloud (production), https: 'https://open-tp.ezrpro.com', http: 'http://open-tp.ezrpro.com'}\n- {name: KOS 测试环境\
  \ (test), https: 'https://open-kos-q1.ezrpro.com', http: null}\n- {name: KOS QCloud (production), https: 'https://open-kos-tp.ezrpro.com', http: null}\ngaps:\n  - No OAuth 2.0, OIDC, or scoped tokens — a single long-lived Token per brand.\n  - No published token rotation or revocation procedure.\n  - Plaintext HTTP endpoints are published alongside HTTPS for the UCloud and QCloud environments.\n  - The Token is never transmitted, which is a genuine strength of the scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezr/refs/heads/main/authentication/ezr-authentication.yml
summary_line: signedRequest · 1 scheme
tags:
- Company
- Enterprise
- SCRM
- CRM
- Retail
- Marketing
- WeChat
- E-Commerce
- Loyalty
- Membership
- Coupons
- Point of Sale
- Webhooks
- China
---
