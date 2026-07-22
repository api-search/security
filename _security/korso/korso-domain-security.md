---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: korsoai.com
  spf: true
hosts:
- cert_expires: Sep 11 00:57:21 2026 GMT
  host: korsoai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Korso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Korso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Korso
provider_slug: korso
slug: korso-domain-security
source_filename: korso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: korsoai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:57:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: korsoai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korso/refs/heads/main/security/korso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Model Context Protocol
- Developer Tools
- Open Source
- Agent Coordination
- Y Combinator
---
