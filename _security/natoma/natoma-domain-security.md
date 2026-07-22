---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: natoma.ai
  spf: true
hosts:
- cert_expires: Sep  4 00:50:53 2026 GMT
  host: natoma.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natoma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natoma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Natoma
provider_slug: natoma
slug: natoma-domain-security
source_filename: natoma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: natoma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:50:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: natoma.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natoma/refs/heads/main/security/natoma-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cybersecurity
- Model Context Protocol
- MCP
- AI Agents
- Identity
- Access Management
- Governance
- Security
---
