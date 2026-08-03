---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: underdogfantasy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: underdogsports.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Sep 30 02:49:50 2026 GMT
  host: www.underdogsports.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 04:25:15 2026 GMT
  host: underdogfantasy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 01:11:46 2026 GMT
  host: app.underdogsports.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 02:31:16 2026 GMT
  host: status.underdogfantasy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:57:28 2026 GMT
  host: api.underdogfantasy.com
  hsts: null
  https: true
  note: non-public mobile/web application backend; returns 404 at the root and for every spec path probed
  tls_version: TLSv1.3
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  note: third-party secondary-market listing host, not operated by Underdog
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Underdog Fantasy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Underdog Fantasy, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Underdog Fantasy
provider_slug: underdog-fantasy
slug: underdog-fantasy-domain-security
source_filename: underdog-fantasy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.underdogsports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:49:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: underdogfantasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:25:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.underdogsports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:11:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.underdogfantasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 02:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.underdogfantasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:57:28 2026 GMT\n  hsts: null\n  note: non-public mobile/web application backend; returns 404 at the root and for\n    every spec path probed\n- host: forgeglobal.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n  note: third-party secondary-market listing host, not operated by Underdog\ndomains:\n- domain: underdogfantasy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: underdogsports.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/underdog-fantasy/refs/heads/main/security/underdog-fantasy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sports
- Fantasy Sports
- Sports Betting
- Prediction Markets
- Gaming
- Entertainment
- Consumer
- Mobile
---
