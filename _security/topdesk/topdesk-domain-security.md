---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: topdesk.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: true
  domain: topdesk.net
  spf: true
hosts:
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: www.topdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 11:00:18 2026 GMT
  host: developers.topdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 03:36:36 2026 GMT
  host: yourcompany.topdesk.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Topdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TOPdesk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TOPdesk
provider_slug: topdesk
slug: topdesk-domain-security
source_filename: topdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.topdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.topdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:00:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourcompany.topdesk.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:36:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: topdesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: topdesk.net\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc:\
  \ false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topdesk/refs/heads/main/security/topdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ITSM
- Enterprise Service Management
- Help Desk
- Incident Management
- Change Management
- Asset Management
---
