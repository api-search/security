---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seated.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seatedapp.io
  spf: true
hosts:
- cert_expires: Sep 18 08:49:51 2026 GMT
  host: www.seated.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: api.seatedapp.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Seated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seated, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seated
provider_slug: seated
slug: seated-domain-security
source_filename: seated-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seated.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:49:51 2026 GMT\n  hsts: false\n- host: api.seatedapp.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: seated.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: seatedapp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seated/refs/heads/main/security/seated-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- live events
- concerts
- ticketing
- artists
- venues
- tour dates
- fan notifications
- presales
- music
- entertainment
---
