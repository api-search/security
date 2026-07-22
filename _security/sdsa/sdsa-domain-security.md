---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sdsa.ai
  spf: true
hosts:
- cert_expires: Aug 23 06:40:40 2026 GMT
  host: sdsa.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sdsa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SDSA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SDSA
provider_slug: sdsa
slug: sdsa-domain-security
source_filename: sdsa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sdsa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:40:40 2026 GMT\n  hsts: false\ndomains:\n- domain: sdsa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sdsa/refs/heads/main/security/sdsa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- AI Agents
- Agentic
- Operating System
- Developer Platform
- Stealth Startup
- Consumer Software
---
