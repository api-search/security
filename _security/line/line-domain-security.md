---
api_specs:
- filename: messaging-api.yml
  format: yaml
  label: LINE Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/messaging-api.yml
- filename: liff.yml
  format: yaml
  label: LINE Front-end Framework (LIFF) Server API
  slug: liff
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/liff.yml
- filename: channel-access-token.yml
  format: yaml
  label: LINE Channel Access Token API
  slug: channel-access-token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/channel-access-token.yml
- filename: insight.yml
  format: yaml
  label: LINE Insight API
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/insight.yml
- filename: manage-audience.yml
  format: yaml
  label: LINE Manage Audience API
  slug: manage-audience
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/manage-audience.yml
- filename: shop.yml
  format: yaml
  label: LINE Shop (Mission Stickers) API
  slug: shop
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/shop.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: line.me
  spf: false
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
- cert_expires: Jul 27 01:41:01 2026 GMT
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
overview: 'Domain security posture for LINE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: LINE
provider_slug: line
slug: line-domain-security
source_filename: line-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: line.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:06:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developers.line.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 01:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.line.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: line.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: line.biz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/security/line-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Chatbots
- Social Login
- Mini Apps
- Marketing
- Japan
---
