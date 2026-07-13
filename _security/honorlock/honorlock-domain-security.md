---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: honorlock.com
  spf: true
hosts:
- cert_expires: Aug 12 05:30:02 2026 GMT
  host: honorlock.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: docs.honorlock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Honorlock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honorlock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Honorlock
provider_slug: honorlock
slug: honorlock-domain-security
source_filename: honorlock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honorlock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 05:30:02 2026 GMT\n  hsts: false\n- host: docs.honorlock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: honorlock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honorlock/refs/heads/main/security/honorlock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Proctoring
- Online Proctoring
- Academic Integrity
- Assessment
- EdTech
- LTI
- Exams
- Education
---
