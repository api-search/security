---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thinkparametric.com
  spf: true
hosts:
- cert_expires: Sep 23 22:40:50 2026 GMT
  host: thinkparametric.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Think Parametric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Think Parametric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Think Parametric
provider_slug: think-parametric
slug: think-parametric-domain-security
source_filename: think-parametric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thinkparametric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:40:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thinkparametric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/think-parametric/refs/heads/main/security/think-parametric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- E-Learning
- Architecture
- Design
- BIM
- Parametric Design
- Professional Certification
- Online Courses
---
