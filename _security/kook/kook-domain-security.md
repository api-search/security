---
api_specs:
- filename: kook-bot-kook-api-openapi.yml
  format: yaml
  label: KOOK 将Bot连接到 KOOK 服务器 API
  slug: kook-bot-kook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kook/openapi/kook-bot-kook-api-openapi.yml
- filename: kook-default-api-openapi.yml
  format: yaml
  label: KOOK 事件通知介绍 API
  slug: kook-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kook/openapi/kook-default-api-openapi.yml
- filename: kook-gateway-api-openapi.yml
  format: yaml
  label: KOOK Gateway接口 API
  slug: kook-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kook/openapi/kook-gateway-api-openapi.yml
- filename: kook-kmarkdown-api-openapi.yml
  format: yaml
  label: KOOK K Markdown与卡片消息 API
  slug: kook-kmarkdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kook/openapi/kook-kmarkdown-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kookapp.cn
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.kookapp.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KOOK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KOOK
provider_slug: kook
slug: kook-domain-security
source_filename: kook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kookapp.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kookapp.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kook/security/kook-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Voice Communication
- Gaming
- Community
- Real-time
---
