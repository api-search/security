---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xiaomishu.com
  spf: true
hosts:
- host: xiaomishu.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''xiaomishu.c'
kind: domain-security
layout: security
method: probed
name: Xiaomishu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiaomishu (订餐小秘书), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Xiaomishu (订餐小秘书)
provider_slug: xiaomishu
slug: xiaomishu-domain-security
source_filename: xiaomishu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xiaomishu.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''xiaomishu.c'\n  hsts: null\ndomains:\n- domain: xiaomishu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaomishu/refs/heads/main/security/xiaomishu-domain-security.yml
summary_line: DMARC
tags:
- Company
- Restaurants
- Reservations
- Dining
- Food
- Shanghai
- China
---
