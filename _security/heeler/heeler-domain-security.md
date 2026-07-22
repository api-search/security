---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heeler.com
  spf: true
hosts:
- cert_expires: Sep 29 11:31:35 2026 GMT
  host: heeler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heeler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heeler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heeler
provider_slug: heeler
slug: heeler-domain-security
source_filename: heeler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heeler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:31:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heeler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heeler/refs/heads/main/security/heeler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Application Security
- DevSecOps
- AI
- Agents
- MCP
- Agent Skills
- Code Security
- Vulnerability Management
- SAST
- SCA
- Secrets Detection
- AI SDLC
---
