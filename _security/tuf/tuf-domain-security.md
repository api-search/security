---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theupdateframework.io
  spf: false
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug 29 09:00:31 2026 GMT
  host: theupdateframework.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: theupdateframework.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tuf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Update Framework (TUF), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: The Update Framework (TUF)
provider_slug: tuf
slug: tuf-domain-security
source_filename: tuf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theupdateframework.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:00:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: theupdateframework.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theupdateframework.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuf/refs/heads/main/security/tuf-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- Cloud Native
- Graduated
- Security
- Software Supply Chain
- Software Updates
- Verification
---
