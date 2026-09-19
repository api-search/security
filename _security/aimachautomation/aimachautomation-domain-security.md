---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: descnc-china.com
  hsts: false
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: desu-aimach.com
  hsts: false
  spf: true
  spf_record: v=spf1 include:spf.qiye.aliyun.com -all
hosts:
- host: descnc-china.com
  http_status: 200
  https: false
  note: HTTP 200 on port 80; no TLS listener on port 443.
- host: www.descnc-china.com
  http_status: 200
  https: false
- host: desu-aimach.com
  https: false
  note: Mail-only domain (MX + SPF, no A record).
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aimachautomation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIMACH Automation, probed live across 3 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AIMACH Automation
provider_slug: aimachautomation
slug: aimachautomation-domain-security
source_filename: aimachautomation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apis.yml website host and the corporate mail domain\nnote: >-\n  The company's only live web host, descnc-china.com, serves plain HTTP and does not\n  answer on port 443 at all — https://descnc-china.com/ returns a connection failure,\n  not a certificate error. The AIMACH-branded domain desu-aimach.com carries MX and\n  SPF records (Alibaba Cloud corporate mail) but no A record, so it is a mail-only\n  domain. CAA absence was re-confirmed directly against 8.8.8.8 after the first probe\n  timed out.\nhosts:\n- host: descnc-china.com\n  https: false\n  http_status: 200\n  note: HTTP 200 on port 80; no TLS listener on port 443.\n- host: www.descnc-china.com\n  https: false\n  http_status: 200\n- host: desu-aimach.com\n  https: false\n  note: Mail-only domain (MX + SPF, no A record).\ndomains:\n- domain: descnc-china.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  hsts: false\n- domain:\
  \ desu-aimach.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.qiye.aliyun.com -all'\n  dmarc: false\n  hsts: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimachautomation/refs/heads/main/security/aimachautomation-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Industrial Automation
- Manufacturing
- Machine Tools
- CNC
- Robotics
- Hardware
- China
---
