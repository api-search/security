---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: continua.ai
  spf: true
hosts:
- cert_expires: Oct  2 20:08:40 2026 GMT
  host: www.continua.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Continua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Continua, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Continua
provider_slug: continua
slug: continua-domain-security
source_filename: continua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.continua.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:08:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: continua.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continua/refs/heads/main/security/continua-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Agents
- Developer Tools
- Coding Agents
- CLI
- Agentic
- Developer OS
---
