---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentnexus.app
  spf: false
hosts:
- cert_expires: Dec 13 08:17:42 2026 GMT
  host: agentnexus.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentnexus App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Nexus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agent Nexus
provider_slug: agentnexus-app
slug: agentnexus-app-domain-security
source_filename: agentnexus-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentnexus.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 08:17:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentnexus.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentnexus-app/security/agentnexus-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Infrastructure
- Registry
- Agents
- Platform
---
