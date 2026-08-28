---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pinger.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: textfree.com
  spf: false
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sideline.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getindex.com
  spf: true
hosts:
- cert_expires: Nov  2 02:17:58 2026 GMT
  host: www.pinger.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:25:02 2026 GMT
  host: textfree.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 05:40:50 2026 GMT
  host: www.sideline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: getindex.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 23 18:58:54 2026 GMT
  host: api.pinger.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: messages.sideline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: app.getindex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinger, probed live across 7 host(s) and 4 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pinger
provider_slug: pinger
slug: pinger-domain-security
source_filename: pinger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 02:17:58 2026 GMT\n  hsts: false\n- host: textfree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.sideline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 05:40:50 2026 GMT\n  hsts: false\n- host: getindex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\n- host: api.pinger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 18:58:54 2026 GMT\n  hsts: false\n- host: messages.sideline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\n- host: app.getindex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n\
  - domain: pinger.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: textfree.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sideline.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getindex.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinger/refs/heads/main/security/pinger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Telecommunications
- Messaging
- SMS
- Voice
- Mobile Applications
- Phone Numbers
- Consumer Applications
- Small Business
---
