---
description: ''
domains:
- caa:
  - 0 issue "telesec.de"
  - 0 issuewild "letsencrypt.org"
  - 128 iodef "mailto:webmaster@berlinonline.net"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: berlin.de
  spf: true
hosts:
- cert_expires: Aug  5 12:51:53 2026 GMT
  host: daten.berlin.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Berlin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City, Berlin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: City, Berlin
provider_slug: city-berlin
slug: city-berlin-domain-security
source_filename: city-berlin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daten.berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 12:51:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: berlin.de\n  dnssec: false\n  caa:\n  - 0 issue \"telesec.de\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 128 iodef \"mailto:webmaster@berlinonline.net\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-berlin/refs/heads/main/security/city-berlin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Public APIs
---
