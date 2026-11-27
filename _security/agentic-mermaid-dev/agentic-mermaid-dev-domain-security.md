---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentic-mermaid.dev
  spf: false
hosts:
- cert_expires: Jan 27 00:53:21 2027 GMT
  host: agentic-mermaid.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentic Mermaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentic Mermaid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agentic Mermaid
provider_slug: agentic-mermaid-dev
slug: agentic-mermaid-dev-domain-security
source_filename: agentic-mermaid-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentic-mermaid.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 00:53:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentic-mermaid.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentic-mermaid-dev/security/agentic-mermaid-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Diagram Generation
- Visualization
- Mermaid
- AI Agents
- CLI
---
