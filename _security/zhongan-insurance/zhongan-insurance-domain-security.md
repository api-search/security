---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zhongan.com
  spf: false
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.zhongan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: open.zhongan.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zhongan Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZhongAn Insurance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ZhongAn Insurance
provider_slug: zhongan-insurance
slug: zhongan-insurance-domain-security
source_filename: zhongan-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zhongan.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.zhongan.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zhongan.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhongan-insurance/refs/heads/main/security/zhongan-insurance-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Digital Insurance
- China
---
