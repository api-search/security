---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: filmai.ai
  spf: true
hosts:
- cert_expires: Feb  3 00:54:46 2027 GMT
  host: filmai.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Filmai Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cinema Master Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cinema Master Pro
provider_slug: filmai-ai
slug: filmai-ai-domain-security
source_filename: filmai-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filmai.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 00:54:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: filmai.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/filmai-ai/security/filmai-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Video
- Film
- Generative AI
- Text to Video
- Storyboard
- Short Drama
- Taiwan
- Creative Tools
- Media Production
---
