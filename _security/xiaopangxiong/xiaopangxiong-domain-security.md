---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 51xpx.com.cn
  mx: false
  note: DNS queries resolved successfully (A records present for apex and www); TXT/SPF, _dmarc TXT, DNSKEY, CAA, and MX answers were all empty — these absences are genuine DNS data, not probe failures.
  spf: false
hosts:
- host: www.51xpx.com.cn
  https: false
  note: TCP 443 connection refused / timed out from US egress (150.158.238.197, China-hosted). Site is live for Chinese visitors (indexed by search engines; Wayback snapshot 2025-02-24 returns 200). TLS/HSTS could not be observed from this vantage point.
- host: mobile.51xpx.com
  https: false
  note: TCP 443 connection refused from US egress (1.116.90.233, Tencent Cloud). Not reachable from this vantage point.
kind: domain-security
layout: security
method: probed
name: Xiaopangxiong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiaopangxiong, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Xiaopangxiong
provider_slug: xiaopangxiong
slug: xiaopangxiong-domain-security
source_filename: xiaopangxiong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probed from US egress)\nhosts:\n- host: www.51xpx.com.cn\n  https: false\n  note: >-\n    TCP 443 connection refused / timed out from US egress (150.158.238.197,\n    China-hosted). Site is live for Chinese visitors (indexed by search\n    engines; Wayback snapshot 2025-02-24 returns 200). TLS/HSTS could not be\n    observed from this vantage point.\n- host: mobile.51xpx.com\n  https: false\n  note: >-\n    TCP 443 connection refused from US egress (1.116.90.233, Tencent Cloud).\n    Not reachable from this vantage point.\ndomains:\n- domain: 51xpx.com.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  mx: false\n  note: >-\n    DNS queries resolved successfully (A records present for apex and www);\n    TXT/SPF, _dmarc TXT, DNSKEY, CAA, and MX answers were all empty — these\n    absences are genuine DNS data, not probe failures.\nnotes: >-\n  Xiaopangxiong's web properties\
  \ are hosted in mainland China and refuse\n  connections from US networks, so HTTPS-layer posture (TLS version, cert,\n  HSTS) is unobservable from this pipeline. DNS-layer posture was fully\n  probed: no DNSSEC, no CAA, no SPF, no DMARC, and no MX on 51xpx.com.cn.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaopangxiong/refs/heads/main/security/xiaopangxiong-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- B2B
- E-Commerce
- Building Materials
- Home Renovation
- Construction
- Logistics
- China
---
