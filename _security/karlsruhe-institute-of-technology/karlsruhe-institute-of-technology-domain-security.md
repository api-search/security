---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kit.edu
  spf: true
hosts:
- cert_expires: Sep 29 21:48:04 2026 GMT
  host: www.kit.edu
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:32:08 2026 GMT
  host: www.bibliothek.kit.edu
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 12:30:10 2026 GMT
  host: dbkit.bibliothek.kit.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karlsruhe Institute Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karlsruhe Institute of Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Karlsruhe Institute of Technology
provider_slug: karlsruhe-institute-of-technology
slug: karlsruhe-institute-of-technology-domain-security
source_filename: karlsruhe-institute-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kit.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:48:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.bibliothek.kit.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:32:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: dbkit.bibliothek.kit.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 12:30:10 2026 GMT\n  hsts: false\ndomains:\n- domain: kit.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karlsruhe-institute-of-technology/refs/heads/main/security/karlsruhe-institute-of-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Research Data
- Library
- Germany
---
