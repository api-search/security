---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prenda.com
  spf: true
hosts:
- cert_expires: Nov 11 00:37:39 2026 GMT
  host: www.prenda.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 07:15:57 2026 GMT
  host: help.prenda.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 01:05:38 2026 GMT
  host: discover.prenda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 00:35:02 2026 GMT
  host: microschools.prenda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prenda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prenda, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Prenda
provider_slug: prenda
slug: prenda-domain-security
source_filename: prenda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of prenda.com and its www/help/discover/microschools hosts\nhosts:\n- host: www.prenda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 00:37:39 2026 GMT\n  hsts: false\n- host: help.prenda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 07:15:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: discover.prenda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:05:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: microschools.prenda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 00:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prenda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nnote: Prenda publishes no API, so there are no OpenAPI servers[] hosts to probe; these are the four live\n  web hosts on prenda.com. www.prenda.com (Webflow) serves no HSTS header while help/discover/microschools\n\
  \  all do. prenda.com has SPF but NO DMARC record at _dmarc.prenda.com (NXDOMAIN on TXT), no DNSSEC and\n  no CAA records.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prenda/refs/heads/main/security/prenda-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Education
- Education Technology
- Microschools
- K-12
- Learning Management
- Curriculum
- School Choice
- Homeschooling
- Design Systems
---
