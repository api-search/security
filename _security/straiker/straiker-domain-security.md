---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: straiker.ai
  spf: true
hosts:
- cert_expires: Oct  3 22:28:10 2026 GMT
  host: www.straiker.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Straiker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Straiker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Straiker
provider_slug: straiker
slug: straiker-domain-security
source_filename: straiker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.straiker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:28:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: straiker.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/straiker/refs/heads/main/security/straiker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Artificial Intelligence
- AI Security
- Agentic AI
- Runtime Security
- LLM Security
- MCP
---
