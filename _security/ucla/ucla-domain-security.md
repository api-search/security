---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ucla.edu
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.ucla.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 16:42:55 2026 GMT
  host: developer.api.ucla.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: digital.library.ucla.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, Los Angeles, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of California, Los Angeles
provider_slug: ucla
slug: ucla-domain-security
source_filename: ucla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucla.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: developer.api.ucla.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  1 16:42:55 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: digital.library.ucla.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ucla.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/security/ucla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Student Information
- Course Catalog
- Library
- IIIF
- United States
- California
---
