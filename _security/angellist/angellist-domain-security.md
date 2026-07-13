---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: angellist.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@wellfound.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wellfound.com
  spf: true
hosts:
- cert_expires: Sep  9 19:39:40 2026 GMT
  host: www.angellist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:17:13 2026 GMT
  host: wellfound.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 08:00:05 2026 GMT
  host: docs.angellist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angellist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AngelList, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AngelList
provider_slug: angellist
slug: angellist-domain-security
source_filename: angellist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angellist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:39:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: wellfound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:17:13 2026 GMT\n  hsts: false\n- host: docs.angellist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:00:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: angellist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wellfound.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@wellfound.com\"\n  spf: true\n  dmarc: true\n \
  \ dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angellist/refs/heads/main/security/angellist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documents
- Funds
- Investing
- Jobs
- Startups
- Transactions
- Venture Capital
---
