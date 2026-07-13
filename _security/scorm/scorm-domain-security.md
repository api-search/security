---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scorm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xapi.com
  spf: true
hosts:
- cert_expires: Aug 15 06:04:25 2026 GMT
  host: scorm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 01:34:04 2026 GMT
  host: xapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scorm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SCORM, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SCORM
provider_slug: scorm
slug: scorm-domain-security
source_filename: scorm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scorm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 06:04:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: xapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scorm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: xapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scorm/refs/heads/main/security/scorm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Learning
- LMS
- Standards
- Education
- Interoperability
---
