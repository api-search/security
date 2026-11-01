---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crowvault.ai
  spf: true
hosts:
- cert_expires: Jan 14 14:44:24 2027 GMT
  host: crowvault.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crowvault Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crowvault-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: crowvault-ai
provider_slug: crowvault-ai
slug: crowvault-ai-domain-security
source_filename: crowvault-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowvault.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:44:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crowvault.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/crowvault-ai/security/crowvault-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- DevTools
- API
- Automation
- Cloud
- Platform
---
