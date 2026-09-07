---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imaginode.ai
  spf: true
hosts:
- cert_expires: Nov  5 11:29:08 2026 GMT
  host: imaginode.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imaginode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imaginode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Imaginode
provider_slug: imaginode
slug: imaginode-domain-security
source_filename: imaginode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imaginode.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 11:29:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: imaginode.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imaginode/refs/heads/main/security/imaginode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ai
- image generation
- video generation
- text to speech
- mcp
- generative ai
- llm
- creative tools
---
