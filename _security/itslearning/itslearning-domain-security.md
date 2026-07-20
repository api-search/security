---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: itslearning.com
  spf: true
hosts:
- cert_expires: Sep  4 02:39:07 2026 GMT
  host: itslearning.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developer.itslearning.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 06:27:49 2026 GMT
  host: eu1.itslearning.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itslearning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for itslearning, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: itslearning
provider_slug: itslearning
slug: itslearning-domain-security
source_filename: itslearning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itslearning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:39:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.itslearning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: eu1.itslearning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:27:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: itslearning.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itslearning/refs/heads/main/security/itslearning-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Saas
- Education
- EdTech
- Learning Management System
- LMS
- LTI
- Norway
---
