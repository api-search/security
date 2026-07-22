---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sett.ai
  spf: true
hosts:
- cert_expires: Oct 15 19:37:27 2026 GMT
  host: www.sett.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sett Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sett AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sett AI
provider_slug: sett-ai
slug: sett-ai-domain-security
source_filename: sett-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sett.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:37:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sett.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sett-ai/refs/heads/main/security/sett-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Mobile Games
- User Acquisition
- Advertising
- Creative
- Agentic AI
---
