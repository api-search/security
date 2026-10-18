---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:webmaster@whatfontis.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: whatfontis.com
  spf: true
hosts:
- cert_expires: Dec 22 12:35:19 2026 GMT
  host: whatfontis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Whatfontis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WhatFontIS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WhatFontIS
provider_slug: whatfontis
slug: whatfontis-domain-security
source_filename: whatfontis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whatfontis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 12:35:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whatfontis.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:webmaster@whatfontis.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whatfontis/refs/heads/main/security/whatfontis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Font Identification
- Artificial Intelligence
- Design Tools
- Typography
---
