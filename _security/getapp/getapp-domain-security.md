---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getapp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gartner.com
  spf: true
hosts:
- cert_expires: Sep  9 23:58:12 2026 GMT
  host: www.getapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 05:00:45 2026 GMT
  host: www.gartner.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetApp, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GetApp
provider_slug: getapp
slug: getapp-domain-security
source_filename: getapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:58:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.gartner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 05:00:45 2026 GMT\n  hsts: null\ndomains:\n- domain: getapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gartner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getapp/refs/heads/main/security/getapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Business Software
- Software Discovery
---
