---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: godmodeai.co
  spf: true
hosts:
- cert_expires: Jan 17 16:39:52 2027 GMT
  host: godmodeai.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Godmodeai Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for godmodeai-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: godmodeai-co
provider_slug: godmodeai-co
slug: godmodeai-co-domain-security
source_filename: godmodeai-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: godmodeai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 16:39:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: godmodeai.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/godmodeai-co/security/godmodeai-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Game Development
- Animation
- Asset Generation
- Sprite Tools
---
