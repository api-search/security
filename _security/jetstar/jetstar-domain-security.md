---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetstar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: navitaire.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.jetstar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:02:49 2026 GMT
  host: apiblog.jetstar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: jqapi.navitaire.com
  https: false
kind: domain-security
layout: security
method: probed
name: Jetstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetstar, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jetstar
provider_slug: jetstar
slug: jetstar-domain-security
source_filename: jetstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\n- host: apiblog.jetstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:02:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jqapi.navitaire.com\n  https: false\ndomains:\n- domain: jetstar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: navitaire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetstar/refs/heads/main/security/jetstar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- Aviation
- Airline
- Low Cost Carrier
- Distribution
- Booking
- GDS
- Corporate Travel
- Qantas Group
---
