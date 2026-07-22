---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qunar.com
  spf: true
hosts:
- cert_expires: Apr  3 09:56:35 2027 GMT
  host: www.qunar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qunar Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qunar Com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Qunar Com
provider_slug: qunar-com
slug: qunar-com-domain-security
source_filename: qunar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qunar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 09:56:35 2027 GMT\n  hsts: false\ndomains:\n- domain: qunar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qunar-com/refs/heads/main/security/qunar-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Travel
- Hotels
- Flights
- Travel Booking
- Travel Search
- Online Travel Agency
- China
---
