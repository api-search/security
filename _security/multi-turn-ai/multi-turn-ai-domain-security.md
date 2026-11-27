---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: multi-turn.ai
  spf: false
hosts:
- cert_expires: Jan 15 19:35:35 2027 GMT
  host: www.multi-turn.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Multi-turn Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Multi-turn Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Multi-turn Inc.
provider_slug: multi-turn-ai
slug: multi-turn-ai-domain-security
source_filename: multi-turn-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.multi-turn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 19:35:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: multi-turn.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/multi-turn-ai/security/multi-turn-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Memory
- Long Term
- South Korea
- Startups
---
