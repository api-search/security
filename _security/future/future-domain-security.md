---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: future.co
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.future.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Future Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Future, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Future
provider_slug: future
slug: future-domain-security
source_filename: future-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.future.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: future.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/future/refs/heads/main/security/future-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Fitness
- Health
- Personal Training
- Coaching
- Wellness
- Mobile App
---
