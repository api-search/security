---
api_specs:
- filename: wechat-webhooks-asyncapi.yml
  format: yaml
  label: WeChat Pay APIv3 (Direct-Connect Merchant)
  slug: wechat-pay-apiv3-direct-merchant
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/asyncapi/wechat-webhooks-asyncapi.yml
- filename: wechat-webhooks-asyncapi.yml
  format: yaml
  label: WeChat Official Accounts API
  slug: wechat-official-accounts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/asyncapi/wechat-webhooks-asyncapi.yml
- filename: wechat-webhooks-asyncapi.yml
  format: yaml
  label: WeChat Work (WeCom) API
  slug: wechat-work-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/asyncapi/wechat-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wechat.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: qq.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.wechat.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: weixin.qq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: pay.weixin.qq.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wechat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeChat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WeChat
provider_slug: wechat
slug: wechat-domain-security
source_filename: wechat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wechat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: weixin.qq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\n- host: pay.weixin.qq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wechat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wechat/refs/heads/main/security/wechat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Social
- Payments
- Mini Programs
- Mini Games
- Official Accounts
- Enterprise Communication
- Cloud Hosting
- Video
- Identity
- China
- Super App
- Tencent
---
