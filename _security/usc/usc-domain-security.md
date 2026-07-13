---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: usc.edu
  spf: true
hosts:
- cert_expires: Sep 14 09:29:38 2026 GMT
  host: www.usc.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- host: web-app.usc.edu
  https: false
kind: domain-security
layout: security
method: probed
name: Usc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Southern California, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Southern California
provider_slug: usc
slug: usc-domain-security
source_filename: usc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:29:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: web-app.usc.edu\n  https: false\ndomains:\n- domain: usc.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usc/refs/heads/main/security/usc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United States
- California
- Courses
---
