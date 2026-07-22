---
description: ''
domains: []
hosts: []
kind: domain-security
layout: security
method: probed
name: Dajiabao Domain Security
name_suffix: Domain Security
overview: Domain security posture for dajiabao, probed live across 0 host(s) and 0 registrable domain(s).
provider_name: dajiabao
provider_slug: dajiabao
slug: dajiabao-domain-security
source_filename: dajiabao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: DNS + TCP/TLS probe of dajiabao.com (api-evangelist enrichment pipeline)\ndomain: dajiabao.com\nreachable: false\nsummary: >-\n  dajiabao.com resolves in DNS but serves no web content. Both TCP/80 and TCP/443\n  time out (connection refused / filtered) from the probe host, so no HTTP, TLS,\n  HSTS, or /.well-known/ surface could be evaluated. Mail is delegated to Tencent\n  Exmail. No email-authentication or certificate-issuance policy records are\n  published.\ndns:\n  a:\n  - 139.196.207.93\n  nameservers:\n  - ns1.ename.net\n  - ns2.ename.net\n  mx:\n  - priority: 5\n    host: mxbiz1.qq.com\n  - priority: 10\n    host: mxbiz2.qq.com\n  dnssec:\n    enabled: false\n    evidence: no DS record at the parent zone\n  caa:\n    present: false\n    evidence: no CAA RRset on dajiabao.com\nregistration:\n  registrar: eName Technology Co., Ltd.\n  created: '2010-07-16'\n  expires: '2028-07-16'\n  status:\n  - clientDeleteProhibited\n\
  \  - clientTransferProhibited\nemail_authentication:\n  spf:\n    present: false\n    evidence: no v=spf1 TXT record on dajiabao.com\n  dmarc:\n    present: false\n    evidence: no TXT record at _dmarc.dajiabao.com\ntransport:\n  https:\n    reachable: false\n    port: 443\n    evidence: TCP connect to 139.196.207.93:443 refused/timed out\n  http:\n    reachable: false\n    port: 80\n    evidence: TCP connect to 139.196.207.93:80 refused/timed out\n  tls: null\n  hsts: null\nwell_known:\n  probed: false\n  evidence: host unreachable over HTTP/HTTPS; /.well-known/ could not be requested\nnotes:\n- The unrelated domain dajiabao.cn (154.89.236.95) serves SEO-spam/adult keyword\n  content and is NOT associated with this company. It was checked and deliberately\n  excluded from this profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dajiabao/refs/heads/main/security/dajiabao-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Venture Backed
- Qiming
- China
- Portfolio Lead
---
