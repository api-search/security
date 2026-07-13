---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: true
  domain: runescape.wiki
  spf: false
hosts:
- cert_expires: Oct  4 22:01:02 2026 GMT
  host: runescape.wiki
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runescape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RuneScape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: RuneScape
provider_slug: runescape
slug: runescape-domain-security
source_filename: runescape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runescape.wiki\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: runescape.wiki\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runescape/refs/heads/main/security/runescape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Games And Comics
- Public APIs
---
