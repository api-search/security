---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gramforge.io
  spf: true
hosts:
- cert_expires: Jan  9 16:30:08 2027 GMT
  host: gramforge.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GramForge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GramForge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GramForge
provider_slug: gramforge-io
slug: gramforge-io-domain-security
source_filename: gramforge-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gramforge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 16:30:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gramforge.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gramforge-io/security/gramforge-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- No-Code
- Telegram
- Chatbots
- Small Business
---
