---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: funfriday.work
  spf: true
hosts:
- cert_expires: Jan  7 01:06:01 2027 GMT
  host: funfriday.work
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fun Friday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fun Friday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fun Friday
provider_slug: funfriday-work
slug: funfriday-work-domain-security
source_filename: funfriday-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: funfriday.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 01:06:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: funfriday.work\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/funfriday-work/security/funfriday-work-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Team Building
- Remote Work
- Online Games
- Icebreaker
- Virtual Events
---
