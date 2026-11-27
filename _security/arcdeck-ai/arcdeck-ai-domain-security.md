---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arcdeck.ai
  spf: true
hosts:
- cert_expires: Jan  4 21:03:07 2027 GMT
  host: arcdeck.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcdeck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcdeck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arcdeck
provider_slug: arcdeck-ai
slug: arcdeck-ai-domain-security
source_filename: arcdeck-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcdeck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 21:03:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arcdeck.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arcdeck-ai/security/arcdeck-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Presentation
- Automation
- Software-as-a-Service
- Productivity
---
