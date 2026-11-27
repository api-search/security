---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groki.meme
  spf: false
hosts:
- cert_expires: Jan 12 10:36:49 2027 GMT
  host: groki.meme
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Groki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Groki
provider_slug: groki-meme
slug: groki-meme-domain-security
source_filename: groki-meme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groki.meme\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 10:36:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: groki.meme\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/groki-meme/security/groki-meme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Meme
- Image Generation
- Face Swap
- Animation
---
