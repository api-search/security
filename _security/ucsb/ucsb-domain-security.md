---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ucsb.edu
  spf: true
hosts:
- cert_expires: Sep 22 18:56:56 2026 GMT
  host: www.ucsb.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 06:59:54 2026 GMT
  host: developer.ucsb.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: alexandria.ucsb.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ucsb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, Santa Barbara, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of California, Santa Barbara
provider_slug: ucsb
slug: ucsb-domain-security
source_filename: ucsb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucsb.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.ucsb.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:59:54 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: alexandria.ucsb.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ucsb.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsb/refs/heads/main/security/ucsb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Student Information System
- Campus
- California
- United States
---
