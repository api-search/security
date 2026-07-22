---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aiva.ai
  spf: true
hosts:
- cert_expires: Sep 30 07:22:31 2026 GMT
  host: aiva.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aiva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aiva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aiva
provider_slug: aiva
slug: aiva-domain-security
source_filename: aiva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiva.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 07:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aiva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiva/refs/heads/main/security/aiva-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Music
- Music Generation
- Generative AI
- Audio
- MIDI
- Creative Tools
- Media
---
