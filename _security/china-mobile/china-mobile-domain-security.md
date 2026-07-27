---
api_specs:
- filename: china-mobile-onenet-studio-openapi.yml
  format: yaml
  label: OneNET Studio Application API
  slug: onenet-studio-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/china-mobile/refs/heads/main/openapi/china-mobile-onenet-studio-openapi.yml
- filename: china-mobile-vcs-openapi.yml
  format: yaml
  label: OneNET Voice Call Service (VCS) API
  slug: onenet-voice-call-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/china-mobile/refs/heads/main/openapi/china-mobile-vcs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chinamobileltd.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: 10086.cn
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: heclouds.com
  spf: false
hosts:
- cert_expires: Jan 23 00:54:37 2027 GMT
  host: www.chinamobileltd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr  1 08:39:04 2027 GMT
  host: dev.10086.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: open.iot.10086.cn
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: openapi.heclouds.com
  hsts: false
  https: true
  note: OneNET open API gateway; returns HTTP 403 to anonymous requests (openresty).
  tls_version: TLSv1.2
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: api.heclouds.com
  hsts: false
  https: true
  note: OneNET legacy device cloud API; anonymous GET /devices returns a token authentication error (nginx).
  tls_version: TLSv1.2
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: iot-api.heclouds.com
  hsts: false
  https: true
  note: OneNET new-generation device API; anonymous requests return code 10403.
  tls_version: TLSv1.2
- host: api.iot.10086.cn
  hsts: false
  https: true
  note: IoT Card Capability Open Platform (Tomcat). TLS version and certificate expiry were not captured in this round.
kind: domain-security
layout: security
method: probed
name: China Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for China Mobile, probed live across 7 host(s) and 3 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: China Mobile
provider_slug: china-mobile
slug: china-mobile-domain-security
source_filename: china-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chinamobileltd.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 00:54:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.10086.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 08:39:04 2027 GMT\n  hsts: false\n- host: open.iot.10086.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: openapi.heclouds.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n  note: OneNET open API gateway; returns HTTP 403 to anonymous requests (openresty).\n- host: api.heclouds.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n  note: OneNET legacy device cloud API; anonymous GET /devices returns a token\n    authentication error (nginx).\n- host: iot-api.heclouds.com\n\
  \  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n  note: OneNET new-generation device API; anonymous requests return code 10403.\n- host: api.iot.10086.cn\n  https: true\n  hsts: false\n  note: IoT Card Capability Open Platform (Tomcat). TLS version and certificate expiry\n    were not captured in this round.\ndomains:\n- domain: chinamobileltd.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: 10086.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: heclouds.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nsummary: >-\n  Every China Mobile host reachable over HTTPS, but the posture is thin. No registrable\n  domain in the estate publishes DNSSEC, a CAA record, an SPF record or a DMARC policy —\n  three domains, zero of twelve controls. HSTS is set only on the corporate site\n  (www.chinamobileltd.com, one year) and the OneNET portal (open.iot.10086.cn, 30 days);\n  none of the four\
  \ API hosts sets it. TLS 1.2 predominates; only dev.10086.cn negotiated\n  TLS 1.3.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/china-mobile/refs/heads/main/security/china-mobile-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Telecommunications
- China
- Mobile Network Operator
- Network APIs
- CAMARA
- GSMA Open Gateway
- IoT
- 5G
- Broadband
- Quality on Demand
- Number Authentication
- Satellite
---
