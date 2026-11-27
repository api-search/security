---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lexpad.app
  spf: true
hosts:
- cert_expires: Feb  2 19:53:44 2027 GMT
  host: lexpad.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lexpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexpad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lexpad
provider_slug: lexpad-app
slug: lexpad-app-domain-security
source_filename: lexpad-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexpad.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 19:53:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lexpad.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lexpad-app/security/lexpad-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vocabulary
- Artificial Intelligence
- Language Learning
- Education
---
