---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hotapi.ai
  spf: true
hosts:
- cert_expires: Jan  3 21:06:02 2027 GMT
  host: hotapi.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hotapi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hotapi-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: hotapi-ai
provider_slug: hotapi-ai
slug: hotapi-ai-domain-security
source_filename: hotapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:06:02 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: hotapi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hotapi-ai/security/hotapi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- NSFW
- Chat
- Image Generation
- Video Generation
- Voice Generation
---
