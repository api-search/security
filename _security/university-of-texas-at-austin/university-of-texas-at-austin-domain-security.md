---
description: ''
domains:
- caa:
  - 0 contactemail "net-tech@its.utexas.edu"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: utexas.edu
  spf: true
hosts:
- cert_expires: Sep  1 17:35:46 2026 GMT
  host: www.utexas.edu
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: repositories.lib.utexas.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:54:10 2026 GMT
  host: guides.lib.utexas.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Texas At Austin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Texas at Austin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Texas at Austin
provider_slug: university-of-texas-at-austin
slug: university-of-texas-at-austin-domain-security
source_filename: university-of-texas-at-austin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.utexas.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:35:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: repositories.lib.utexas.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n- host: guides.lib.utexas.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:54:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: utexas.edu\n  dnssec: false\n  caa:\n  - 0 contactemail \"net-tech@its.utexas.edu\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-texas-at-austin/refs/heads/main/security/university-of-texas-at-austin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Data
- Institutional Repository
- United States
- Texas
---
