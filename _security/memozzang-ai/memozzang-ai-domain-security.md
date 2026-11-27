---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memozzang.ai
  spf: true
hosts:
- cert_expires: Dec 29 08:40:23 2026 GMT
  host: memozzang.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 메모짱 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 메모짱, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 메모짱
provider_slug: memozzang-ai
slug: memozzang-ai-domain-security
source_filename: memozzang-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memozzang.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:40:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memozzang.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/memozzang-ai/security/memozzang-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Collaboration
- Artificial Intelligence
- Productivity
- Family
---
