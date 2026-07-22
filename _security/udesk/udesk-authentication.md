---
api_key_in:
- query
auth_types:
- signature
- bearer
- jwt-sso
description: Udesk publishes no OpenAPI, so this profile is captured from the developer docs rather than derived from securitySchemes. Every Udesk API family uses signed-request authentication (HMAC-style digest signatures computed over the admin email + API token + timestamp), not OAuth. There is no OAuth2 / OIDC surface, hence no scopes/ artifact for this provider.
kind: authentication
layout: security
method: searched
name: Udesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Udesk secures its APIs with signature, bearer, and jwt-sso across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Udesk
provider_slug: udesk
scheme_count: 7
schemes:
- api: Udesk Open API v2
  detail: 'sign=SHA256(email&open_api_token&timestamp&nonce&sign_version), passed as query params email, timestamp, sign, nonce, sign_version=v2 on https://[subdomain].udesk.cn/open_api_v1/*. The docs note SHA-1 as a fallback when SHA-256 fails. The open_api_token is obtained by POST /log_in with the super-admin email and password. Anti-replay: timestamp must be within 5 minutes; nonce is single-use within 15 minutes. Failure returns code 2059 ("open api签名不对").'
  docs: https://www.udesk.cn/doc/apiv2/intro/
  in: query
  name: open-api-v2-signature
  type: signature
- api: Udesk Open API v1 (legacy)
  detail: sign=MD5(QueryString + "&" + Secret) where Secret is the SSO shared secret from the admin console. The docs themselves flag this as a security weakness ("V1 版本的接口存在安全隐患") and recommend migrating to v2.
  docs: https://www.udesk.cn/doc/apiv1/intro/
  in: query
  name: open-api-v1-signature
  type: signature
- api: Udesk Robot (KM) API
  detail: sign=SHA1(email&api_token&timestamp) on https://km.udesk.cn/api/v1/*; api_token comes from the KM console (管理-系统设置-秘钥). Default timestamp expiry five minutes.
  docs: https://www.udesk.cn/doc/robot/intro/
  in: query
  name: robot-km-signature
  type: signature
- api: ServiceGo API
  detail: sign=SHA1(email&api_token&timestamp) for tenants created before 2021-06-03, sign=SHA256(email&api_token&timestamp) for tenants created after; on https://servicego.udesk.cn/api/v1/*.
  docs: https://www.udesk.cn/doc/sercive/general-instructions/
  in: query
  name: servicego-signature
  type: signature
- api: KCS knowledge API
  detail: 'POST /api/auth/open/token with appId (tenant identifier) + userId returns a token used as "Authorization: Bearer {token}" on https://{tenant_kcs_domain}/api/sdk/*. Tokens expire every 50 minutes.'
  docs: https://www.udesk.cn/doc/kcs/kcs-intro/
  name: kcs-bearer
  scheme: bearer
  type: http
- api: ServiceGo single sign-on
  detail: SSO uses HS256-signed JWTs (header {"alg":"HS256","typ":"JWT"}, payload aud=U_SERVICE, sub=email-or-job-number) signed with the tenant secret, presented to /backend/auth/users/{accessKeyId}. SAML/OAuth/LDAP are only available through the separate OneInto product.
  docs: https://www.udesk.cn/doc/sercive/sso/
  name: servicego-sso-jwt
  type: jwt
- api: Robot webhook (outbound calls to customer endpoints)
  detail: Message-triggered webhooks sign with SHA1(integrationName&appKey&timestamp); task-push webhooks sign with md5Hex(key + taskNodeId + sessionId + timestamp).
  docs: https://www.udesk.cn/doc/robot/webhook/
  name: robot-webhook-signature
  type: signature
slug: udesk-authentication
source_filename: udesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.udesk.cn/doc/apiv2/intro/\ndocs: https://www.udesk.cn/doc/apiv2/intro/\ndescription: >-\n  Udesk publishes no OpenAPI, so this profile is captured from the developer\n  docs rather than derived from securitySchemes. Every Udesk API family uses\n  signed-request authentication (HMAC-style digest signatures computed over\n  the admin email + API token + timestamp), not OAuth. There is no OAuth2 /\n  OIDC surface, hence no scopes/ artifact for this provider.\nsummary:\n  types: [signature, bearer, jwt-sso]\n  oauth2_flows: []\n  api_key_in: [query]\nschemes:\n  - name: open-api-v2-signature\n    api: Udesk Open API v2\n    type: signature\n    in: query\n    docs: https://www.udesk.cn/doc/apiv2/intro/\n    detail: >-\n      sign=SHA256(email&open_api_token&timestamp&nonce&sign_version), passed as\n      query params email, timestamp, sign, nonce, sign_version=v2 on\n      https://[subdomain].udesk.cn/open_api_v1/*.\
  \ The docs note SHA-1 as a\n      fallback when SHA-256 fails. The open_api_token is obtained by POST\n      /log_in with the super-admin email and password. Anti-replay: timestamp\n      must be within 5 minutes; nonce is single-use within 15 minutes. Failure\n      returns code 2059 (\"open api签名不对\").\n  - name: open-api-v1-signature\n    api: Udesk Open API v1 (legacy)\n    type: signature\n    in: query\n    docs: https://www.udesk.cn/doc/apiv1/intro/\n    detail: >-\n      sign=MD5(QueryString + \"&\" + Secret) where Secret is the SSO shared\n      secret from the admin console. The docs themselves flag this as a\n      security weakness (\"V1 版本的接口存在安全隐患\") and recommend migrating\n      to v2.\n  - name: robot-km-signature\n    api: Udesk Robot (KM) API\n    type: signature\n    in: query\n    docs: https://www.udesk.cn/doc/robot/intro/\n    detail: >-\n      sign=SHA1(email&api_token&timestamp) on https://km.udesk.cn/api/v1/*;\n      api_token comes from the KM console (管理-系统设置-秘钥).\
  \ Default\n      timestamp expiry five minutes.\n  - name: servicego-signature\n    api: ServiceGo API\n    type: signature\n    in: query\n    docs: https://www.udesk.cn/doc/sercive/general-instructions/\n    detail: >-\n      sign=SHA1(email&api_token&timestamp) for tenants created before\n      2021-06-03, sign=SHA256(email&api_token&timestamp) for tenants created\n      after; on https://servicego.udesk.cn/api/v1/*.\n  - name: kcs-bearer\n    api: KCS knowledge API\n    type: http\n    scheme: bearer\n    docs: https://www.udesk.cn/doc/kcs/kcs-intro/\n    detail: >-\n      POST /api/auth/open/token with appId (tenant identifier) + userId\n      returns a token used as \"Authorization: Bearer {token}\" on\n      https://{tenant_kcs_domain}/api/sdk/*. Tokens expire every 50 minutes.\n  - name: servicego-sso-jwt\n    api: ServiceGo single sign-on\n    type: jwt\n    docs: https://www.udesk.cn/doc/sercive/sso/\n    detail: >-\n      SSO uses HS256-signed JWTs (header {\"alg\":\"HS256\"\
  ,\"typ\":\"JWT\"}, payload\n      aud=U_SERVICE, sub=email-or-job-number) signed with the tenant secret,\n      presented to /backend/auth/users/{accessKeyId}. SAML/OAuth/LDAP are only\n      available through the separate OneInto product.\n  - name: robot-webhook-signature\n    api: Robot webhook (outbound calls to customer endpoints)\n    type: signature\n    docs: https://www.udesk.cn/doc/robot/webhook/\n    detail: >-\n      Message-triggered webhooks sign with SHA1(integrationName&appKey&timestamp);\n      task-push webhooks sign with md5Hex(key + taskNodeId + sessionId + timestamp).\nnotes:\n  - All APIs are designed for server-side calling only; the docs warn that\n    calling from web/mobile clients risks leaking the auth token.\n  - API signing is also advertised on the security page (\"签名使用SHA2/AES256\n    等强壮的安全算法\") at https://www.udesk.cn/product_safety_features.html.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/udesk/refs/heads/main/authentication/udesk-authentication.yml
summary_line: signature/bearer/jwt-sso · 7 schemes
tags:
- Company
- Enterprise
- Customer Service
- Call Center
- Ticketing
- Chatbots
- CRM
- Knowledge Management
- SaaS
- China
---
