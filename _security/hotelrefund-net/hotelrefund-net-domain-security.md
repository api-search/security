---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hotelrefund.net
  spf: true
hosts:
- cert_expires: Jan 26 08:01:20 2027 GMT
  host: hotelrefund.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HotelRefund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HotelRefund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HotelRefund
provider_slug: hotelrefund-net
slug: hotelrefund-net-domain-security
source_filename: hotelrefund-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotelrefund.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 08:01:20 2027 GMT\n  hsts: false\ndomains:\n- domain: hotelrefund.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hotelrefund-net/security/hotelrefund-net-domain-security.yml
summary_line: TLSv1.3
tags:
- Hotel Price Tracking
---
