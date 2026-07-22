---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nextacademy.com
  spf: true
hosts:
- cert_expires: Aug 28 17:21:26 2026 GMT
  host: nextacademy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Next Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NEXT Academy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NEXT Academy
provider_slug: next-academy
slug: next-academy-domain-security
source_filename: next-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:21:26 2026 GMT\n  hsts: false\ndomains:\n- domain: nextacademy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-academy/refs/heads/main/security/next-academy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Coding Bootcamp
- Developer Training
- EdTech
- Software Engineering
- Southeast Asia
---
