---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: osu.edu
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.osu.edu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: library.osu.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 14 23:08:08 2026 GMT
  host: kb.osu.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ohio State University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ohio State University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ohio State University
provider_slug: ohio-state-university
slug: ohio-state-university-domain-security
source_filename: ohio-state-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: library.osu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: kb.osu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 23:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: osu.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohio-state-university/refs/heads/main/security/ohio-state-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Institutional Repository
- Open Access
- United States
---
