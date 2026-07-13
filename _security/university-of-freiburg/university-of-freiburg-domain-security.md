---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uni-freiburg.de
  spf: true
hosts:
- cert_expires: Oct 20 07:43:22 2026 GMT
  host: www.uni-freiburg.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:32:34 2026 GMT
  host: freidok.uni-freiburg.de
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 08:24:02 2026 GMT
  host: www.ub.uni-freiburg.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Freiburg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Freiburg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: University of Freiburg
provider_slug: university-of-freiburg
slug: university-of-freiburg-domain-security
source_filename: university-of-freiburg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uni-freiburg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 07:43:22 2026 GMT\n  hsts: false\n- host: freidok.uni-freiburg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:32:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.ub.uni-freiburg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 08:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uni-freiburg.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-freiburg/refs/heads/main/security/university-of-freiburg-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Germany
---
