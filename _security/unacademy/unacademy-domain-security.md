---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unacademy.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: unacademy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unacademy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unacademy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unacademy
provider_slug: unacademy
slug: unacademy-domain-security
source_filename: unacademy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: unacademy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unacademy/refs/heads/main/security/unacademy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edtech
- Education
- Learning
- Exam Preparation
- Courses
- India
---
