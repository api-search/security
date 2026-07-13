---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: umich.edu
  spf: true
hosts:
- cert_expires: Aug 19 21:56:27 2026 GMT
  host: umich.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 16:34:00 2026 GMT
  host: www.lib.umich.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 21:41:28 2026 GMT
  host: its.umich.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Michigan Ann Arbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Michigan-Ann Arbor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Michigan-Ann Arbor
provider_slug: university-of-michigan-ann-arbor
slug: university-of-michigan-ann-arbor-domain-security
source_filename: university-of-michigan-ann-arbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umich.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:56:27 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.lib.umich.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:34:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: its.umich.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:41:28 2026 GMT\n  hsts: null\ndomains:\n- domain: umich.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-michigan-ann-arbor/refs/heads/main/security/university-of-michigan-ann-arbor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Data
- Institutional Repository
- United States
---
