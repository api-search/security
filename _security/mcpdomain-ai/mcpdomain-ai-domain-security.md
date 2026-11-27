---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcpdomain.ai
  spf: true
hosts:
- cert_expires: Jan  4 18:04:38 2027 GMT
  host: mcpdomain.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCPDomain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPDomain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MCPDomain
provider_slug: mcpdomain-ai
slug: mcpdomain-ai-domain-security
source_filename: mcpdomain-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpdomain.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 18:04:38 2027 GMT\n  hsts: false\ndomains:\n- domain: mcpdomain.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcpdomain-ai/security/mcpdomain-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Domain Registrar
- AI Agents
- Email Forwarding
- Domain Transfer
- OpenSRS
---
