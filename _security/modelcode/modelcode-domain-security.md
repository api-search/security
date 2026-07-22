---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelcode.ai
  spf: true
hosts:
- cert_expires: Oct  2 19:04:21 2026 GMT
  host: modelcode.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modelcode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modelcode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Modelcode
provider_slug: modelcode
slug: modelcode-domain-security
source_filename: modelcode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modelcode.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: modelcode.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelcode/refs/heads/main/security/modelcode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Code Modernization
- Legacy Migration
- Developer Tools
- Software Engineering
- AI Agents
- DevOps
---
