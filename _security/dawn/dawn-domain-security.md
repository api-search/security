---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dawn.health
  spf: true
hosts:
- cert_expires: Aug 18 03:05:06 2026 GMT
  host: dawn.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dawn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dawn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dawn
provider_slug: dawn
slug: dawn-domain-security
source_filename: dawn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dawn.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:05:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dawn.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dawn/refs/heads/main/security/dawn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Digital Health
- Healthcare
- Sleep
- Insomnia
- CBT-I
- Telehealth
- Mental Health
- Consumer Health
---
