---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rex.com.au
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rexflyer.com.au
  note: No TXT records at all at the apex — so no SPF — and no _dmarc record. The loyalty domain publishes no email authentication of any kind.
  spf: false
hosts:
- cert_expires: Feb 28 03:38:34 2027 GMT
  host: www.rex.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: ibe2.rex.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Internet booking engine. Root returned HTTP 500 to a HEAD request at probe time.
  tls_version: TLSv1.3
- host: mbe.rex.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: Manage My Booking. HTTP 200.
  tls_version: TLSv1.3
- host: flights.rex.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: EveryMundo / AirTRFX fare-marketing pages. HTTP/2, returned 405 to a HEAD request. Strongest transport posture of any Rex host — and it is a vendor's stack, not Rex's own.
  tls_version: TLSv1.3
- host: www.rexflyer.com.au
  hsts: false
  https: true
  note: Rex Flyer loyalty. Only host still negotiating TLS 1.2 rather than 1.3.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rex Airlines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rex Airlines, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rex Airlines
provider_slug: rex-airlines
slug: rex-airlines-domain-security
source_filename: rex-airlines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every host published in apis.yml\nnote: >-\n  Rex publishes no OpenAPI and no API host, so the hosts probed here are the\n  public web properties named in apis.yml — the marketing site, the internet\n  booking engine, manage-my-booking, the EveryMundo/AirTRFX fare-page host and\n  the Rex Flyer loyalty site. Absence of a record (no CAA, no HSTS, no DNSSEC)\n  is recorded as measured, not inferred.\nhosts:\n- host: www.rex.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 03:38:34 2027 GMT\n  hsts: false\n- host: ibe2.rex.com.au\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 2592000\n  note: Internet booking engine. Root returned HTTP 500 to a HEAD request at probe time.\n- host: mbe.rex.com.au\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 2592000\n  note: Manage My Booking. HTTP 200.\n- host: flights.rex.com.au\n  https: true\n  tls_version:\
  \ TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    EveryMundo / AirTRFX fare-marketing pages. HTTP/2, returned 405 to a HEAD\n    request. Strongest transport posture of any Rex host — and it is a vendor's\n    stack, not Rex's own.\n- host: www.rexflyer.com.au\n  https: true\n  tls_version: TLSv1.2\n  hsts: false\n  note: Rex Flyer loyalty. Only host still negotiating TLS 1.2 rather than 1.3.\ndomains:\n- domain: rex.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rexflyer.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    No TXT records at all at the apex — so no SPF — and no _dmarc record. The\n    loyalty domain publishes no email authentication of any kind.\nfindings:\n- HSTS is absent on the primary www host and on the loyalty host.\n- No CAA records on either registrable domain.\n- No DNSSEC on either registrable domain.\n- rex.com.au\
  \ publishes DMARC but at p=none (monitor only, no enforcement).\n- rexflyer.com.au publishes neither SPF nor DMARC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rex-airlines/refs/heads/main/security/rex-airlines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- Aviation
- Airline
- Regional Aviation
- Distribution
- Booking
- Corporate Travel
- Loyalty
- Freight
---
