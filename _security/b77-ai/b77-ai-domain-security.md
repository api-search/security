---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: b77.ai
  spf: true
hosts:
- cert_expires: Jan 17 11:52:37 2027 GMT
  host: b77.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: B77 Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for b77-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: b77-ai
provider_slug: b77-ai
slug: b77-ai-domain-security
source_filename: b77-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: b77.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 11:52:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: b77.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/b77-ai/security/b77-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Automation
- Enterprise
- Productivity
- Private
---
