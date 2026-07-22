---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:ops@kayak.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kayak.com
  spf: true
hosts:
- cert_expires: Sep 27 09:42:45 2026 GMT
  host: www.kayak.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kayak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kayak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kayak
provider_slug: kayak
slug: kayak-domain-security
source_filename: kayak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kayak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:42:45 2026 GMT\n  hsts: null\ndomains:\n- domain: kayak.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:ops@kayak.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayak/refs/heads/main/security/kayak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Metasearch
- Flights
- Hotels
- Car Rental
- Travel Search
- Price Comparison
- Booking Holdings
- AI
---
