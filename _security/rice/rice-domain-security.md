---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rice.edu
  spf: true
hosts:
- cert_expires: Jul 28 22:07:52 2026 GMT
  host: www.rice.edu
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:04:49 2026 GMT
  host: repository.rice.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: library.rice.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rice University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rice University
provider_slug: rice
slug: rice-domain-security
source_filename: rice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rice.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 22:07:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: repository.rice.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:04:49 2026 GMT\n  hsts: false\n- host: library.rice.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rice.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/security/rice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Repository
- United States
---
