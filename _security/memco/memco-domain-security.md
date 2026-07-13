---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memco.ai
  spf: true
hosts:
- cert_expires: Oct  2 01:52:03 2026 GMT
  host: www.memco.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Memco
provider_slug: memco
slug: memco-domain-security
source_filename: memco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.memco.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:52:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memco.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memco/refs/heads/main/security/memco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI
- Knowledge Management
- Memory
---
