---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fabhotels.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.fabhotels.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fabhotels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FabHotels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FabHotels
provider_slug: fabhotels
slug: fabhotels-domain-security
source_filename: fabhotels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fabhotels.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: fabhotels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabhotels/refs/heads/main/security/fabhotels-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Travel
- Hospitality
- Hotels
- Booking
- India
---
