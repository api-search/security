---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reservaturno.com
  spf: true
hosts:
- cert_expires: Sep 29 23:44:04 2026 GMT
  host: reservaturno.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Y And S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Y&S, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Y&S
provider_slug: y-and-s
slug: y-and-s-domain-security
source_filename: y-and-s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reservaturno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:44:04 2026 GMT\n  hsts: null\ndomains:\n- domain: reservaturno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/y-and-s/refs/heads/main/security/y-and-s-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Booking
- Appointments
- Beauty
- Wellness
- Argentina
- Consumer
---
