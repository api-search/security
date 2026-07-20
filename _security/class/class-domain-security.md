---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: class.com
  spf: true
hosts:
- cert_expires: Aug 20 18:22:22 2026 GMT
  host: www.class.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Class Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Class, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Class
provider_slug: class
slug: class-domain-security
source_filename: class-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.class.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:22:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: class.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class/refs/heads/main/security/class-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Edtech
- Education
- Virtual Classroom
- Learning
- LMS
- Video Conferencing
- Live Learning
---
