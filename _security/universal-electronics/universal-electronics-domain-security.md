---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uei.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quicksetcloud.com
  spf: true
hosts:
- cert_expires: Oct 15 17:08:21 2026 GMT
  host: www.uei.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 18:09:00 2026 GMT
  host: quicksetcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universal Electronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universal Electronics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Universal Electronics
provider_slug: universal-electronics
slug: universal-electronics-domain-security
source_filename: universal-electronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uei.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:08:21 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: quicksetcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:09:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uei.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: quicksetcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universal-electronics/refs/heads/main/security/universal-electronics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Smart Home
- IoT
- Device Control
- Consumer Electronics
- Entertainment
- Climate Control
- Remote Controls
---
