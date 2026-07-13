---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brown.edu
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iiif.io
  spf: true
hosts:
- cert_expires: Sep 25 12:44:20 2026 GMT
  host: www.brown.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:14:32 2026 GMT
  host: repository.library.brown.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: iiif.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brown University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brown University
provider_slug: brown
slug: brown-domain-security
source_filename: brown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brown.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: repository.library.brown.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:14:32 2026 GMT\n  hsts: false\n- host: iiif.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brown.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: iiif.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brown/refs/heads/main/security/brown-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Digital Repository
- IIIF
- United States
---
