---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botrista.com
  spf: true
- caa: []
  dmarc: true
  dmarc_pct: 20
  dmarc_policy: quarantine
  dnssec: false
  domain: botrista.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: botrista.info
  spf: false
hosts:
- cert_expires: Oct 23 00:24:37 2026 GMT
  host: botrista.com
  hsts: false
  https: true
  note: responds HTTP 202 with an sgcaptcha interstitial to non-browser clients; every path including /robots.txt and /.well-known/* is gated behind the challenge
  tls_version: TLSv1.3
- cert_expires: Oct 24 05:34:14 2026 GMT
  host: www.botrista.info
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: botrista.io
  hsts: false
  https: true
  note: same sgcaptcha interstitial as botrista.com
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: cloudbar.botrista.io
  hsts: false
  https: true
  note: CloudBar operator web application (nginx behind CloudFront)
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: portal.botrista.com
  hsts: false
  https: true
  note: Botrista Data Portal web application (nginx behind CloudFront)
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: us-orderbws.botrista.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: private application backend for CloudBar; api.botrista.io 307-redirects here
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Botrista Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botrista, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Botrista
provider_slug: botrista
slug: botrista-domain-security
source_filename: botrista-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the Botrista application hosts\n  discovered during contract discovery (cloudbar.botrista.io, portal.botrista.com,\n  us-orderbws.botrista.io)\nhosts:\n- host: botrista.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 00:24:37 2026 GMT\n  hsts: false\n  note: responds HTTP 202 with an sgcaptcha interstitial to non-browser clients; every\n    path including /robots.txt and /.well-known/* is gated behind the challenge\n- host: www.botrista.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 05:34:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: botrista.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n  note: same sgcaptcha interstitial as botrista.com\n- host: cloudbar.botrista.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\n  note:\
  \ CloudBar operator web application (nginx behind CloudFront)\n- host: portal.botrista.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\n  note: Botrista Data Portal web application (nginx behind CloudFront)\n- host: us-orderbws.botrista.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: private application backend for CloudBar; api.botrista.io 307-redirects here\ndomains:\n- domain: botrista.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: botrista.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 20\n- domain: botrista.info\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\nx-evidence:\n  fetched: '2026-08-02'\n  method: dig (TXT/CAA/DS) plus TLS handshake and HTTP HEAD per host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botrista/refs/heads/main/security/botrista-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Beverage
- Food Service
- Automation
- Restaurant Technology
- IoT
- Hardware
---
