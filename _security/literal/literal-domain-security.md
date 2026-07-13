---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: false
  dnssec: false
  domain: literal.club
  spf: true
hosts:
- cert_expires: Sep 19 21:14:41 2026 GMT
  host: literal.club
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Literal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Literal Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Literal Club
provider_slug: literal
slug: literal-domain-security
source_filename: literal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: literal.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:14:41 2026 GMT\n  hsts: false\ndomains:\n- domain: literal.club\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/literal/refs/heads/main/security/literal-domain-security.yml
summary_line: TLSv1.3
tags:
- Books
- Reading
- Social
- GraphQL
- Book Tracking
- Reading Lists
- Shelves
- Reviews
- Highlights
- Reading Goals
- Book Clubs
- Recommendations
---
