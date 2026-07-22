---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pingxx.com
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.pingxx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: docs.pingxx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.pingxx.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ping++, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ping++
provider_slug: ping
slug: ping-domain-security
source_filename: ping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pingxx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: docs.pingxx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: api.pingxx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pingxx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ping/refs/heads/main/security/ping-domain-security.yml
summary_line: TLSv1.2
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
