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
  domain: kayak.com
  spf: true
hosts:
- cert_expires: Sep 27 09:42:45 2026 GMT
  host: www.kayak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kayak Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KAYAK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KAYAK
provider_slug: kayak-com
slug: kayak-com-domain-security
source_filename: kayak-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kayak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:42:45 2026 GMT\n  hsts: false\ndomains:\n- domain: kayak.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayak-com/refs/heads/main/security/kayak-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Meta Search
- Travel Meta Search
- Flights
- Hotels
- Cars
- Vacation Packages
- Cruises
- Affiliate Network
- White Label
- Deep Links
- Booking Holdings
---
