---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justclip.ai
  spf: true
hosts:
- cert_expires: Jan  1 18:26:04 2027 GMT
  host: justclip.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JustClip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustClip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JustClip
provider_slug: justclip-ai
slug: justclip-ai-domain-security
source_filename: justclip-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justclip.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 18:26:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: justclip.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/justclip-ai/security/justclip-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Clipping
- Social Media
---
