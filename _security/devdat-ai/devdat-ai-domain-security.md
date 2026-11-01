---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: devdat.ai
  spf: false
hosts:
- cert_expires: Dec 29 16:18:37 2026 GMT
  host: www.devdat.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devdat Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevDat.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DevDat.ai
provider_slug: devdat-ai
slug: devdat-ai-domain-security
source_filename: devdat-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.devdat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 16:18:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: devdat.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/devdat-ai/security/devdat-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data
- Platform
- AI
- Integration
- Singapore
---
