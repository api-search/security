---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: promptlens.io
  spf: true
hosts:
- cert_expires: Jan 11 05:36:57 2027 GMT
  host: promptlens.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptlens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PromptLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PromptLens
provider_slug: promptlens
slug: promptlens-domain-security
source_filename: promptlens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptlens.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 05:36:57 2027 GMT\n  hsts: false\ndomains:\n- domain: promptlens.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/promptlens/security/promptlens-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Monitoring
- Testing
- LLM
- Observability
---
