---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: latrobe.edu.au
  spf: true
hosts:
- cert_expires: Oct 26 15:01:57 2026 GMT
  host: www.latrobe.edu.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.latrobe.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: opal.latrobe.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Trobe University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Trobe University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: La Trobe University
provider_slug: la-trobe-university
slug: la-trobe-university-domain-security
source_filename: la-trobe-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.latrobe.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 15:01:57 2026 GMT\n  hsts: null\n- host: api.latrobe.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opal.latrobe.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: latrobe.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-trobe-university/refs/heads/main/security/la-trobe-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Australia
- Victoria
- Research
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Open Access
---
