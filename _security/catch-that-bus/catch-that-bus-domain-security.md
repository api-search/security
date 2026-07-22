---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: catchthatbus.com
  spf: false
hosts:
- cert_expires: Aug 22 07:39:44 2026 GMT
  host: catchthatbus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catch That Bus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catch that bus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Catch that bus
provider_slug: catch-that-bus
slug: catch-that-bus-domain-security
source_filename: catch-that-bus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catchthatbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:39:44 2026 GMT\n  hsts: null\ndomains:\n- domain: catchthatbus.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catch-that-bus/refs/heads/main/security/catch-that-bus-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Transportation
- Bus
- Ticketing
- Travel
- Booking
- Malaysia
---
