---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chipp.ai
  spf: true
hosts:
- cert_expires: Jan  7 00:34:22 2027 GMT
  host: chipp.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chipp Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chipp-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: chipp-ai
provider_slug: chipp-ai
slug: chipp-ai-domain-security
source_filename: chipp-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chipp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 00:34:22 2027 GMT\n  hsts: false\ndomains:\n- domain: chipp.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chipp-ai/security/chipp-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Automation
- SaaS
- HIPAA
- SOC2
---
