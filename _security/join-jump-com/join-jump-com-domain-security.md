---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: join-jump.com
  spf: true
hosts:
- cert_expires: Jan  4 06:34:34 2027 GMT
  host: join-jump.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Join Jump Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jump, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jump
provider_slug: join-jump-com
slug: join-jump-com-domain-security
source_filename: join-jump-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: join-jump.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 06:34:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: join-jump.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/join-jump-com/security/join-jump-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Portage Salarial
- Freelance
- Consulting
---
