---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: fangtek.com.cn
  mx: []
  nameservers:
  - n1.xundns.com
  - n2.xundns.com
  spf: false
hosts:
- a:
  - 154.220.7.201
  host: fangtek.com.cn
  hsts: null
  http_error: empty reply from server
  http_status: null
  https: false
  https_error: TLSV1_ALERT_UNRECOGNIZED_NAME
  resolves: true
  tls_version: null
- a:
  - 154.220.7.201
  host: www.fangtek.com.cn
  hsts: null
  http_error: empty reply from server
  http_status: null
  https: false
  https_error: TLSV1_ALERT_UNRECOGNIZED_NAME
  resolves: true
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Fangtek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FangTek, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FangTek
provider_slug: fangtek
slug: fangtek-domain-security
source_filename: fangtek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + curl probe of fangtek.com.cn (2026-07-20)\nnotes: >-\n  The registered domain resolves, but no reachable web service was observed from\n  the probe location. HTTPS terminates with a TLS \"unrecognized_name\" (SNI) alert\n  and plain HTTP returns an empty reply. No mail or email-authentication records\n  are published. Absence of records is recorded data, not an inferred failure.\nhosts:\n  - host: fangtek.com.cn\n    resolves: true\n    a: [154.220.7.201]\n    https: false\n    https_error: TLSV1_ALERT_UNRECOGNIZED_NAME\n    http_status: null\n    http_error: empty reply from server\n    tls_version: null\n    hsts: null\n  - host: www.fangtek.com.cn\n    resolves: true\n    a: [154.220.7.201]\n    https: false\n    https_error: TLSV1_ALERT_UNRECOGNIZED_NAME\n    http_status: null\n    http_error: empty reply from server\n    tls_version: null\n    hsts: null\ndomains:\n  - domain: fangtek.com.cn\n    nameservers: [n1.xundns.com,\
  \ n2.xundns.com]\n    dnssec: false\n    caa: []\n    mx: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\nwell_known:\n  - {path: /.well-known/security.txt, status: null, error: connection failed}\n  - {path: /.well-known/openid-configuration, status: null, error: connection failed}\n  - {path: /.well-known/oauth-authorization-server, status: null, error: connection failed}\n  - {path: /.well-known/api-catalog, status: null, error: connection failed}\n  - {path: /.well-known/ai-plugin.json, status: null, error: connection failed}\n  - {path: /llms.txt, status: null, error: connection failed}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fangtek/refs/heads/main/security/fangtek-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Semiconductors
- Integrated Circuits
- Analog
- Mixed Signal
- Audio
- Power Management
- Consumer Electronics
- Hardware
- China
---
