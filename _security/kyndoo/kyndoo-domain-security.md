---
description: ''
domains:
- caa: []
  created: '2018-06-26'
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: kyndoo.com
  expires: '2027-06-26'
  mail_provider: Google Workspace
  mx:
  - aspmx.l.google.com
  - alt1.aspmx.l.google.com
  - alt2.aspmx.l.google.com
  - alt3.aspmx.l.google.com
  - alt4.aspmx.l.google.com
  nameservers:
  - ns-1386.awsdns-45.org
  - ns-1617.awsdns-10.co.uk
  - ns-469.awsdns-58.com
  - ns-825.awsdns-39.net
  registrar: GoDaddy.com, LLC
  spf: false
  txt:
  - MS=ms68894663
hosts:
- address: 35.209.23.179
  evidence: connection timed out on both 80 and 443
  host: kyndoo.com
  hsts: null
  http: false
  https: false
  port_443: closed
  port_80: closed
  reachable: false
  tls_version: null
- address: 54.190.94.109
  evidence: connection timed out on 443
  host: www.kyndoo.com
  hsts: null
  http: false
  https: false
  port_443: closed
  reachable: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Kyndoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyndoo, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kyndoo
provider_slug: kyndoo
slug: kyndoo-domain-security
source_filename: kyndoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: dig + TLS/HTTP probe of kyndoo.com and www.kyndoo.com\nnote: >-\n  Kyndoo was acquired by CIPIO (cipio.ai) and the kyndoo.com web property has\n  been taken offline. DNS still resolves and mail (Google Workspace) is still\n  configured, but no HTTP/HTTPS listener answers on either the apex or www.\n  Absence of records below is recorded data, not a gap in the probe.\nhosts:\n  - host: kyndoo.com\n    address: 35.209.23.179\n    https: false\n    http: false\n    port_443: closed\n    port_80: closed\n    reachable: false\n    tls_version: null\n    hsts: null\n    evidence: connection timed out on both 80 and 443\n  - host: www.kyndoo.com\n    address: 54.190.94.109\n    https: false\n    http: false\n    port_443: closed\n    reachable: false\n    tls_version: null\n    hsts: null\n    evidence: connection timed out on 443\ndomains:\n  - domain: kyndoo.com\n    registrar: GoDaddy.com, LLC\n    created: '2018-06-26'\n    expires:\
  \ '2027-06-26'\n    nameservers:\n      - ns-1386.awsdns-45.org\n      - ns-1617.awsdns-10.co.uk\n      - ns-469.awsdns-58.com\n      - ns-825.awsdns-39.net\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    txt:\n      - MS=ms68894663\n    mx:\n      - aspmx.l.google.com\n      - alt1.aspmx.l.google.com\n      - alt2.aspmx.l.google.com\n      - alt3.aspmx.l.google.com\n      - alt4.aspmx.l.google.com\n    mail_provider: Google Workspace\nwell_known_probe:\n  note: >-\n    All /.well-known/ discovery endpoints were probed on both hosts and none\n    were reachable (connection failure, not a 404). No WellKnown or SecurityTxt\n    artifact is claimed for this provider.\n  documents:\n    - path: /.well-known/security.txt\n      status: 0\n      result: unreachable\n    - path: /.well-known/openid-configuration\n      status: 0\n      result: unreachable\n    - path: /.well-known/oauth-authorization-server\n      status: 0\n      result: unreachable\n\
  \    - path: /.well-known/api-catalog\n      status: 0\n      result: unreachable\n    - path: /.well-known/ai-plugin.json\n      status: 0\n      result: unreachable\n    - path: /llms.txt\n      status: 0\n      result: unreachable\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyndoo/refs/heads/main/security/kyndoo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Influencer Marketing
- Marketing
- Social Media
- Advertising
- Customer Data Platform
- Analytics
- Acquired
---
