---
api_specs:
- filename: line-messaging-api-openapi.yml
  format: yaml
  label: LINE Messaging API
  slug: line-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-messaging-api-openapi.yml
- filename: line-webhook-openapi.yml
  format: yaml
  label: LINE Messaging API Webhook
  slug: line-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-webhook-openapi.yml
- filename: line-channel-access-token-openapi.yml
  format: yaml
  label: LINE Channel Access Token API
  slug: line-channel-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-channel-access-token-openapi.yml
- filename: line-insight-openapi.yml
  format: yaml
  label: LINE Insight API
  slug: line-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-insight-openapi.yml
- filename: line-manage-audience-openapi.yml
  format: yaml
  label: LINE Manage Audience API
  slug: line-manage-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-manage-audience-openapi.yml
- filename: line-liff-openapi.yml
  format: yaml
  label: LIFF Server API
  slug: line-liff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-liff-openapi.yml
- filename: line-module-openapi.yml
  format: yaml
  label: LINE Module API
  slug: line-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-module-openapi.yml
- filename: line-module-attach-openapi.yml
  format: yaml
  label: LINE Module Attach API
  slug: line-module-attach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-module-attach-openapi.yml
- filename: line-shop-openapi.yml
  format: yaml
  label: LINE Mission Sticker API
  slug: line-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-shop-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: line.me
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: line.biz
  spf: false
hosts:
- cert_expires: Sep 11 01:06:02 2026 GMT
  host: line.me
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 01:06:25 2027 GMT
  host: developers.line.biz
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.line.me
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Line Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LINE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LINE
provider_slug: line
slug: line-domain-security
source_filename: line-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: line.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:06:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developers.line.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 01:06:25 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.line.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: line.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: line.biz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/security/line-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Chatbots
- Social Login
- Mini Apps
- Marketing
- Webhooks
- OpenID Connect
- Audience
- Analytics
- Japan
---
