---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mit.edu
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.mit.edu
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.2
- host: developers-dev.mit.edu
  https: false
kind: domain-security
layout: security
method: probed
name: Mit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MIT, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MIT
provider_slug: mit
slug: mit-domain-security
source_filename: mit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mit.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 600\n- host: developers-dev.mit.edu\n  https: false\ndomains:\n- domain: mit.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mit/refs/heads/main/security/mit-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- Identity
- Research
- Roles
- University
---
