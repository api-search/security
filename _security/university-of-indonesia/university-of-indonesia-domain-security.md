---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ui.ac.id
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.ui.ac.id
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 11:16:40 2026 GMT
  host: scholarhub.ui.ac.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 04:55:45 2026 GMT
  host: sso.ui.ac.id
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Indonesia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Indonesia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Indonesia
provider_slug: university-of-indonesia
slug: university-of-indonesia-domain-security
source_filename: university-of-indonesia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ui.ac.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n- host: scholarhub.ui.ac.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sso.ui.ac.id\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 04:55:45 2026 GMT\n  hsts: false\ndomains:\n- domain: ui.ac.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-indonesia/refs/heads/main/security/university-of-indonesia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Indonesia
- Research
- Repository
- OAI-PMH
- Authentication
---
