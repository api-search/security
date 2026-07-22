---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: magic.dev
  spf: true
hosts:
- cert_expires: Aug 13 22:25:12 2026 GMT
  host: magic.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Magic
provider_slug: magic-dev
slug: magic-dev-domain-security
source_filename: magic-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magic.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 22:25:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: magic.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-dev/refs/heads/main/security/magic-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- AGI Research
- Coding Agent
- Long Context
- LLM
- Frontier Lab
- No Public API
---
