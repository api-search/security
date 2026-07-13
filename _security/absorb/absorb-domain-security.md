---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myabsorb.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: docs.myabsorb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: rest.myabsorb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Absorb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Absorb LMS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Absorb LMS
provider_slug: absorb
slug: absorb-domain-security
source_filename: absorb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.myabsorb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: rest.myabsorb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: myabsorb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absorb/refs/heads/main/security/absorb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LMS
- Learning Management
- E-Learning
- Training
- Courses
- Enrollments
- Certificates
---
