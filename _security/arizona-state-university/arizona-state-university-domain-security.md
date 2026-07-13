---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "emsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asu.edu
  spf: true
hosts:
- cert_expires: Aug 31 13:47:57 2026 GMT
  host: www.asu.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 21:42:22 2026 GMT
  host: dataverse.asu.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:43:22 2026 GMT
  host: lib.asu.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arizona State University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arizona State University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arizona State University
provider_slug: arizona-state-university
slug: arizona-state-university-domain-security
source_filename: arizona-state-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:47:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dataverse.asu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:42:22 2026 GMT\n  hsts: null\n- host: lib.asu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:43:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asu.edu\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"emsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arizona-state-university/refs/heads/main/security/arizona-state-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- United States
- Arizona
---
